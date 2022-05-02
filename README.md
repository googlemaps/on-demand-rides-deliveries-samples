# On-Demand Rides and Deliveries Samples

## Introduction

The [On-demand Rides and Deliveries (ODRD) Solution](https://developers.google.com/maps/documentation/transportation-logistics/on-demand-rides-deliveries-solution)
is a development toolkit for building on-demand mobility solutions. The
On-demand Rides and Deliveries Samples provide reference implementations of the
various integrations and applications that use the ODRD Solution. You can use
these samples to create, update, and simulate vehicles and trips. These apps
work for both mobile and web.

## Getting Started

Each component of the ODRD Solution resides in its own repository. You can
download the source code from all the repositories via Git submodules by running
the following command.

```
git clone --recursive https://github.com/googlemaps/on-demand-rides-deliveries-samples
```

Note that you must use the `--recursive` flag.

Refer to each component's repository for instructions.

## Components

There are four components to the sample applications:

1.  **The provider backend**, a Java-based server using the Fleet Engine API,
    which supports services for the mobile apps and the web app.

    The source code for the provider backend is located in another repository at
    https://github.com/googlemaps/java-on-demand-rides-deliveries-stub-provider.
    You can access it in this repository through the Git submodule.

2.  **The Driver app**, a mobile app for drivers. It is written using the Driver
    SDK and the Navigation SDK. It communicates with the provider backend to
    obtain matched trips and shows the data in a user interface that allows the
    driver to navigate to waypoints on the trips. The Driver SDK automatically
    sends location updates to Fleet Engine.

    The Driver app can be run on real mobile devices and emulators.
    It is available on two operating systems.

    -   Android: The Driver app for Android is available in Java and Kotlin.
        It is located in another repository at
        https://github.com/googlemaps/android-on-demand-rides-deliveries-samples.
        You can access it in this repository through the Git submodule.

    -   iOS: The Driver app for iOS is available in Swift and Objective-C.
        It is located in another repository at
        https://github.com/googlemaps/ios-on-demand-rides-deliveries-samples.
        You can access it in this repository through the Git submodule.

3.  **The Consumer app**, a mobile app for consumers or riders. It is written
    using the Consumer SDK. It communicates with the provider backend to create
    a trip. It uses the Consumer SDK to retrieve from Fleet Engine the route,
    trip status, ETA, remaining distance, and the driver's location and displays
    them on a map

    The Consumer app can be run on real mobile devices and emulators. It is
    available on two operating systems.

    -   Android: The Consumer app for Android is available in Java and Kotlin.
        It is located in another repository at
        https://github.com/googlemaps/android-on-demand-rides-deliveries-samples.
        You can access it in this repository through the Git submodule.

    -   iOS: The Consumer app for iOS is available in Swift and Objective-C.
        It is located in another repository at
        https://github.com/googlemaps/ios-on-demand-rides-deliveries-samples.
        You can access it in this repository through the Git submodule.

4.  **The web app**, an Angular-based app that can be used in concert with the
    mobile apps to track trips in a web browser. This component is optional.

    The source code for the web app is located in another repository at
    https://github.com/googlemaps/angular-on-demand-rides-deliveries-samples.
    You can access it in this repository through the Git submodule.

## License

```
Copyright 2022 Google LLC.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements.  See the NOTICE file distributed with this work for
additional information regarding copyright ownership.  The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License.  You may obtain a copy of
the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
License for the specific language governing permissions and limitations under
the License.
```
