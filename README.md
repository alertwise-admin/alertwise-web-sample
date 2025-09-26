# AlertWise Web SDK - Sample Application

This repository contains a sample web application that demonstrates how to integrate and use the [AlertWise Web SDK](https://alertwise.net) for sending web push notifications. It provides clear, commented code examples for common use cases.

## Features Demonstrated

This sample application covers the following AlertWise Web SDK features:

*   **SDK Initialization**: How to initialize the AlertWise SDK in your web page.
*   **Subscription Management**: Subscribing and unsubscribing users from push notifications.
*   **Subscriber ID**: Retrieving the unique AlertWise subscriber ID.
*   **Segments**: Adding subscribers to and removing them from segments for targeted messaging.
*   **Tags**: Adding, updating, and removing key-value tags for detailed subscriber segmentation.
*   **Subscriber Properties**: Setting and removing custom data attributes for a subscriber.
*   **Event Logging**: Listening to and logging various SDK events like `onSubscribe`, `onUnsubscribe`, and notification interactions.

## Getting Started

Follow these instructions to get the demo running on your local machine.

### Prerequisites

Because web push notifications and Service Workers require a secure context, you cannot run this demo by simply opening the `index.html` file in your browser. You will need a local web server to serve the files.

Here are a few simple ways to start a local server:

*   **Using Node.js (with `http-server` package):**
    ```sh
    # Install it globally if you haven't already
    npm install -g http-server
    # Run the server
    http-server
    ```

*   **Using VS Code:**
    Install the Live Server extension and click "Go Live" from the editor's status bar.

### Configuration

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/alertwise-admin/alertwise-web-sample.git
    cd alertwise-web-sample
    ```

2.  **Update Credentials (Optional):**
    This demo comes pre-configured with a demo `appId`. To use your own AlertWise application, open `index.html` and replace the placeholder credentials in the SDK initialization script with your own from the AlertWise dashboard.

    ```javascript
    // C:/Users/sintu/git/alertwise-web-sample/index.html

    alertwise.push(["init", {
        appId: "YOUR_APP_ID", // Replace with your App ID
        applicationServerPublicKey: "YOUR_APPLICATION_SERVER_PUBLIC_KEY" // Replace with your VAPID Public Key
    }]);
    ```

### Running the Demo

1.  Start your local web server from the root of the project directory.
2.  Open your browser and navigate to `http://localhost:8000` (or the port your server is running on).
3.  Use the UI to interact with the different features of the AlertWise SDK and see the event logs in real-time.

## Useful Links

Here are some helpful links to learn more about AlertWise and connect with our community:

### Product & Platform
*   [AlertWise Platform](https://alertwise.net/)
*   [Features](https://alertwise.net/features)
*   [Pricing](https://alertwise.net/pricing)
*   [Testimonials](https://alertwise.net/testimonials)
*   [Login to your Account](https://app.alertwise.net/#/login)
*   [Get Started for Free](https://app.alertwise.net/#/signup)

### Documentation & Resources
*   [Documentation](https://documentation.alertwise.net/)
*   [Blog](https://blog.alertwise.net/)
*   [Community Q&A](https://blog.alertwise.net/questions/)
*   [Video Tutorials](https://www.youtube.com/@Alertwisenotification)
*   [FAQs](https://documentation.alertwise.net/faqs/faqs/)
*   [Glossary](https://blog.alertwise.net/glossary/)

### Connect with Us
*   [GitHub](https://github.com/alertwise-admin)
*   [Twitter/X](https://x.com/AlertWisePush)
*   [YouTube](https://www.youtube.com/@Alertwisenotification)

## License

This project is licensed under the MIT License - see the LICENSE file for details.
