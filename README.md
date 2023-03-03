*visnet-docs.github.io*
=====================


## Introduction:

Welcome to the documentation for our [ViSNET AI](https://visnetai.co/) application! In this document, we will provide an overview of the AI application, its purpose, and its capabilities. We will also outline the different components that make up the application and provide instructions on how to use them.

Our AI application is designed to provide users with intelligent and automated solutions to complex problems. It uses advanced algorithms and machine learning techniques to analyze data and provide insights and recommendations to users.

The application is divided into several modules, each designed to handle specific tasks. The modules work together seamlessly to provide a cohesive user experience. The modules include data ingestion, data preprocessing, model training, model validation, and inference.

To use the application, users will need to provide data that the application can analyze. The data should be in a structured format, and users will need to follow specific guidelines for data formatting and cleaning. Once the data is ingested into the application, the data preprocessing module will clean and transform the data into a format suitable for model training.

The model training module uses advanced machine learning algorithms to train models on the cleaned data. The module provides users with a wide range of algorithms to choose from, and users can experiment with different algorithms to find the best fit for their data.

Once a model has been trained, the model validation module will test the model on a set of validation data to ensure that it is accurate and reliable. The module provides users with detailed metrics to help them evaluate the model's performance.

Finally, the inference module allows users to use the trained model to make predictions on new data. The module is designed to be user-friendly, and users can input new data into the module and receive predictions quickly and accurately.

We hope this documentation provides a comprehensive overview of our AI application and its capabilities. If you have any questions or need assistance using the application, please do not hesitate to contact our support team.

## Architecture:

<iframe width="980" height="768" src="https://miro.com/app/live-embed/uXjVPhofS_U=/?moveToViewport=-885,-496,1865,1328&embedId=296968678081&embedAutoplay=true" frameborder="0" scrolling="no" allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen></iframe>

## Tech Stack:

*Frontend:*
The client side of the application is built upon `Next.JS` which is framework on top of React.JS. Next.JS supports pre-rendering, code-splitting, inbuilt routing, it is incredibly fast and brings in many optimizing techniches to make the application fast and reliable.

*Backend:*
The server side of the application is built on Python with `FastAPI` framework. FastAPI is a RESTful web framework for building high performant, robust and production ready web server with Python.

*Microservices:*
The `Drone structural inspection` detects concrete surface defects on drone imagery. Visnet leverages advancements in AI and uses state-of-the-art instance segmentation model `YoloV8` and optimized for the present usecase.

*Cloud service:*
Visnet use open-source framework `BentoML` for model packaging and deployment purpose, also `AWS` cloud services like `EC2,S3` for cloud hosting and storage purposes.


## Guide to getting started:

For developers, to get started clone this repository using the below git command.

<code>git clone https://github.com/visnetai/visnet-frontend-interface.git</code>

Navigate to the local repository and run the following command in the terminal to install all the dependencies.

<code>npm install</code>

To start the development server of the application run the below command in the terminal.

<code>npm run dev</code>

## Userflow:

For detailed view of the app userflow please follow the below presentation.

<iframe width="980" height="768" src="https://miro.com/app/live-embed/uXjVPhCOrcc=/?moveToViewport=-2333,-1246,1433,1035&embedId=360744919598&embedAutoplay=true" frameborder="0" scrolling="no" allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen></iframe>

## Best Practices:

* *Modularised styles:* With `Next.JS` we have the ability to split the css styles into modules and can be used alongside global styles.
* *Reusability(Components):* Visnet application is split into reusable UI components. With the usage of components the application is modularised and is built with little code and is consistent across all the pages.
* *Fonts and styles:* Visnet application contains single font family and the font styles are consistent across the pages.
* *Comments:* Meaningful comments are added in the codebase wherever necessary.
* *Clean codebase:* Visnet codebase is maintained in such a way that all the unnecessary code and the comments are removed so that the bundle size wont be impacted.
* *Minimal usage of packages:* Visnet application is built with minimal usage of third party libraries and packages to avoid dpendency issues and unknown bugs.
* *Optimized Images:* `Next.JS` brings optimization with Next `next/image` component, by default this next/image component uses browser native lazy loading, which may fallback to eager loading for older browsers before Safari 15.4. Next.Js Image have the blur-up placeholder which can be used while the image is loading.
* *Dynamic Imports:* For better performance dynamic imports of components which takes time to load at the initial rendering of the application. With the combination of lazy loading and dynamic imports Visnet got over `90%` score in `lighthouse` analysis.
* *Strong Authorizatrion:* Visnet uses two level authentication with the combination of `jwt tokens` and `SHA-256` algorithm leveraging Next.JS server-side-rendering while eliminating any unthorized access.
* *Prevented content flashing:* With the usage of Nxt.JS server-side-authentication Visnet eliminated unauthorized content flashing.
* *Pre-fetching pages:* With Next.JS Visnet leveraged the prefetching of pages which reduces the FCP time of the application.
* *Limited server calls:* With the usage of react hooks the number of API calls are minimized and the load on the server is balanced.

## Components used:

The components that are used to build Visnet are as follows:
* CustomInputField
* PinField
* CustomButton
* CustomLoader
* NavigationMenu
* Recharts
* SkeletonLoader
* ImageThumbnail
* Modal
* ImageCarousal
* Map
