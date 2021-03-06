.. _add-aws-mobile-hosting-and-streaming:

############################################
Add Hosting and Streaming to Your Mobile App
############################################


.. meta::
   :description: Integrating hosting and streaming


.. _add-aws-mobile-hosting-and-streaming-overview:

Hosting and Streaming
=====================


The Hosting and Streaming feature enables you to host code and content in the cloud for your web,
native mobile, or hybrid app. A simple sample web app that accesses AWS services is deployed when you
enable this feature.

|AMH| creates a container for your content using an `Amazon S3 <http://docs.aws.amazon.com/AmazonS3/latest/dev/>`_ bucket. The content is available publicly on the Internet and you can preview the content directly using a testing URL.

Your content is automatically distributed to a global content delivery network (CDN). `Amazon
CloudFront <https://aws.amazon.com/cloudfront/>`_ also supports media file streaming. To learn more, see `CloudFront Streaming Tutorials <http://docs.aws.amazon.com/mobile-hub/latest/developerguide/url-cf-dev;Tutorials.html>`_.


.. _add-aws-mobile-hosting-and-streaming-back-end-setup:

Set Up Your Backend
===================


.. container:: option

   Android - Java
      #. Complete the :ref:`add-aws-mobile-sdk-basic-setup` steps before using the integration steps on this page.

      #. Use |AMHlong| to deploy your backend in minutes.


         #. Sign in to the `Mobile Hub console <https://console.aws.amazon.com/mobilehub/home/>`_.

         #. Choose :guilabel:`Create a new project`, type a name for it, and then choose
            :guilabel:`Create project`.

            Or select an existing project.

         #. Choose the :guilabel:`Hosting and Streaming` tile.


            #. Choose the :ref:`hosting-and-streaming` feature.

               .. image:: images/add-aws-mobile-add-hosting-and-streaming.png
                  :scale: 100
                  :alt: Image of choosing Hosting and Streaming in the |AMH| console.

               .. only:: pdf

                  .. image:: images/add-aws-mobile-add-hosting-and-streaming.png
                     :scale: 50

               .. only:: kindle

                  .. image:: images/add-aws-mobile-add-hosting-and-streaming.png
                     :scale: 75

            #. Check the box to indicate you understand that content hosted by the feature is
               public, and then choose :guilabel:`Enable`.


               .. image:: images/add-aws-mobile-add-hosting-and-streaming-enable.png
                  :scale: 100
                  :alt: Image of the |AMH| console.

               .. only:: pdf

                  .. image:: images/add-aws-mobile-add-hosting-and-streaming-enable.png
                     :scale: 50

               .. only:: kindle

                  .. image:: images/add-aws-mobile-add-hosting-and-streaming-enable.png
                     :scale: 75

         #. Download your |AMH| project configuration file.

               #. In the |AMH| console, choose your project, and then choose the :guilabel:`Integrate` icon on the left.

               #. Choose :guilabel:`Download Configuration File` to get the :file:`awsconfiguration.json` file that connects your app to your backend.

                  .. image:: images/add-aws-mobile-sdk-download-configuration-file.png
                     :scale: 100 %
                     :alt: Image of the Mobile Hub console when choosing Download Configuration File.

                  .. only:: pdf

                     .. image:: images/add-aws-mobile-sdk-download-nosql-cloud-logic.png
                        :scale: 50

                  .. only:: kindle

                     .. image:: images/add-aws-mobile-sdk-download-nosql-cloud-logic.png
                        :scale: 75

                  *Remember:*

                  Each time you change the |AMH| project for your app, download and use an updated :file:`awsconfiguration.json` to reflect those changes in your app. If NoSQL Database or Cloud Logic are changed, also download and use updated files for those features.

   iOS - Swift
      #. Complete the :ref:`add-aws-mobile-sdk-basic-setup` steps before using the integration steps on this page.

      #. Deploy your AWS services in minutes using |AMHlong|.


         #. Sign in to the `Mobile Hub console <https://console.aws.amazon.com/mobilehub/home/>`_.

         #. Choose :guilabel:`Create a new project`, type a name for it, and then choose
            :guilabel:`Create project`.

            Or select an existing project.

         #. Choose the :guilabel:`Hosting and Streaming` tile.


            #. Choose the :ref:`hosting-and-streaming` feature.

               .. image:: images/add-aws-mobile-add-hosting-and-streaming.png
                  :scale: 100
                  :alt: Image of the |AMH| console.

               .. only:: pdf

                  .. image:: images/add-aws-mobile-add-hosting-and-streaming.png
                     :scale: 50

               .. only:: kindle

                  .. image:: images/add-aws-mobile-add-hosting-and-streaming.png
                     :scale: 75

            #. Check the box to indicate you understand that content hosted by the feature is
               public, and then choose :guilabel:`Enable`.


               .. image:: images/add-aws-mobile-add-hosting-and-streaming-enable.png
                  :scale: 100
                  :alt: Image of the |AMH| console.

               .. only:: pdf

                  .. image:: images/add-aws-mobile-add-hosting-and-streaming-enable.png
                     :scale: 50

               .. only:: kindle

                  .. image:: images/add-aws-mobile-add-hosting-and-streaming-enable.png
                     :scale: 75

         #. Download your |AMH| project configuration file.

               #. In the |AMH| console, choose your project, and then choose the :guilabel:`Integrate` icon on the left.

               #. Choose :guilabel:`Download Configuration File` to get the :file:`awsconfiguration.json` file that connects your app to your backend.

                  .. image:: images/add-aws-mobile-sdk-download-configuration-file.png
                     :scale: 100 %
                     :alt: Image of the Mobile Hub console when choosing Download Configuration File.

                  .. only:: pdf

                     .. image:: images/add-aws-mobile-sdk-download-nosql-cloud-logic.png
                       :scale: 50

                  .. only:: kindle

                     .. image:: images/add-aws-mobile-sdk-download-nosql-cloud-logic.png
                       :scale: 75

                  *Remember:*

                  Each time you change the |AMH| project for your app, download and use an updated :file:`awsconfiguration.json` to reflect those changes in your app. If NoSQL Database or Cloud Logic are changed, also download and use updated files for those features.


   JavaScript
      #. Complete the :ref:`add-aws-mobile-sdk-basic-setup` steps before proceeding on this page.

      #. View the Hosting and Streaming Sample App

         The |AMH| Hosting and Streaming feature creates a sample JavaScript web app that
         demonstrates connecting to the AWS resources of your |AMH| project.

         The sample app web assets are deployed to an |S3| bucket. The bucket is configured to host
         static web content for public access.


         #. In the `Mobile Hub console <https://console.aws.amazon.com/mobilehub/home/>`_, open your project and then choose the Hosting and Streaming tile.

         #. Choose :guilabel:`View from S3`.

            This opens a browser and displays the :file:`index.html` of the sample web app from the
            |S3| bucket.

            .. image:: images/add-aws-mobile-add-hosting-and-streaming-view-from-s3.png
               :scale: 100
               :alt: Image of the |AMH| console.

            .. only:: pdf

               .. image:: images/add-aws-mobile-add-hosting-and-streaming-view-from-s3.png
                  :scale: 50

            .. only:: kindle

               .. image:: images/add-aws-mobile-add-hosting-and-streaming-view-from-s3.png
                  :scale: 75

      **About the Hosting and Streaming Sample App**

      .. note::

         When you enable Hosting and Streaming, |AMH| provisions content in the root of your
         source bucket which includes a local copy of the |JSBlong|
         (:file:`aws-min.js`).


         * :file:`aws-sdk.min.js` - An |JSBlong| source file.

         * :file:`aws-config.js,`- A web app configuration file that is generated to contain
           constants for the endpoints for each |AMH| feature you have enabled for this
           project.

         * `index.html` - Which uses a constant formed in :file:`aws-config.js` to request and
           display an AWS guest (unauthenticated) user identity ID from the |COG| service.

         When you enable Hosting and Streaming an |CFlong| global content delivery network (CDN)
         distribution is created and associated with your bucket. When |AMH| propagates the sample
         web app content to the bucket, the content is then propagated to the CDN and becomes
         available from local endpoints around the globe. If you configure `CloudFront streaming
         <http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Tutorials.html>`_, then media content you upload to your |S3| bucket can be streamed from
         those endpoints.



.. _add-aws-mobile-hosting-and-streaming-app:

Add |AMH| Hosting and Streaming to Your App
===========================================


Use the following steps to add |AMH| Hosting and Streaming to your app.

.. container:: option

   Android - Java
      #. Set up AWS Mobile SDK components with the following :ref:`add-aws-mobile-sdk-basic-setup` steps.


         #. :file:`AndroidManifest.xml` must contain:

            .. code-block:: xml
               :emphasize-lines: 0

                <uses-permission android:name="android.permission.INTERNET" />
                <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
                <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />

         #. :file:`app/build.gradle` must contain:

            .. code-block:: none
               :emphasize-lines: 2

                dependencies{
                    compile 'com.amazonaws:aws-android-sdk-s3:2.6.+'
                }

      #. Add the backend service configuration file to your app.

         #. Right-click your app's :file:`res` folder, and then choose :guilabel:`New > Android
            Resource Directory`. Select :guilabel:`raw` in the :guilabel:`Resource type` dropdown
            menu.

            .. image:: images/add-aws-mobile-sdk-android-studio-res-raw.png
               :scale: 100
               :alt: Image of selecting a Raw Android Resource Directory in Android Studio.

            .. only:: pdf

               .. image:: images/add-aws-mobile-sdk-android-studio-res-raw.png
                  :scale: 50

            .. only:: kindle

               .. image:: images/add-aws-mobile-sdk-android-studio-res-raw.png
                  :scale: 75

         #. From the location where configuration files were downloaded in a previous step, drag
            :file:`awsconfiguration.json` into the :file:`res/raw` folder.


   iOS - Swift
      #. Set up AWS Mobile SDK components with the following :ref:`add-aws-mobile-sdk-basic-setup` steps.


         #. :file:`Podfile` that you configure to install the AWS Mobile SDK must contain:

            .. code-block:: none

                platform :ios, '9.0'

                target :'YOUR-APP-NAME' do
                  use_frameworks!

                      pod 'AWSS3', '~> 2.6.6'    # For file transfers
                      pod 'AWSCognito', '~> 2.6.6'    #For data sync
                      # other pods

                end

            Run :code:`pod install --repo-update` before you continue.

         #. Classes that call |S3| APIs must use the following import statements:

            .. code-block:: none

                import AWSCore
                import AWSS3

      #. Add your backend service configuration to the app.

         From the location where your |AMH| configuration file was downloaded in a previous step,
         drag :file:`awsconfiguration.json` into the folder containing your :file:`info.plist` file
         in your Xcode project.

         Select :guilabel:`Copy items if needed` and :guilabel:`Create groups`, if these options are offered.


   JavaScript
      Use the following options to deploy your web app to hosting, once you have it running in your
      local environment.

      .. _sync-files-with-S3:

      **Upload your Javascript web app assets to S3**

      .. note:: When you upload your web app to the |S3| bucket that |AMH| created, that location
         acts as the source, or origin, for your |CF| CDN endpoints. You can choose from a variety
         of ways to manage your web app assets through use of the Amazon S3 console, the AWS Command
         Line Interface (CLI) or one of the many third party applications available.

         #. Use the |S3| console to manage your web assets

            #. In the `Mobile Hub console <https://console.aws.amazon.com/mobilehub>`_, open your project and choose the Hosting and Streaming tile.

            #. Choose :guilabel:`Manage files`.

               .. image:: images/add-aws-mobile-add-hosting-and-streaming-manage-files.png
                  :scale: 100
                  :alt: Image of the |AMH| console.

               .. only:: pdf

                  .. image:: images/add-aws-mobile-add-hosting-and-streaming-manage-files.png
                     :scale: 50

               .. only:: kindle

                  .. image:: images/add-aws-mobile-add-hosting-and-streaming-manage-files.png
                     :scale: 75

            #. Use the |S3| console user interface to manage your app files.

               .. image:: images/add-aws-mobile-s3-console.png
                  :scale: 100
                  :alt: Image of the |AMH| console.

               .. only:: pdf

                  .. image:: images/add-aws-mobile-s3-console.png
                     :scale: 50

               .. only:: kindle

                  .. image:: images/add-aws-mobile-s3-console.png
                     :scale: 75

         #. Use |CLI|

            The |CLI| allows you to review, upload, move or delete the files stored in your bucket
            using the command line.

            To install and configure the |CLI| client, see `Getting Set Up with the AWS Command Line
            Interface <http://docs.aws.amazon.com/cli/latest/userguide/cli-chap-get-set-up.html>`_

            As an example, the sync command enables transfer of files to and from your local folder
            and your bucket.

            .. code-block:: bash

                $ aws s3 sync <source> <target> [--options]

            The following command syncs all files from your current local folder to the folder in
            your web app's bucket, defined by :code:`path`.

            .. code-block:: bash

                $  aws s3 sync . s3://my-web-app-bucket/path

            To learn more about using |CLI| to manage |S3|, see `Using Amazon S3 with the AWS
            Command Line Interface. <http://docs.aws.amazon.com/cli/latest/userguide/cli-s3.html>`_

      .. _configure-custom-domain:

      **Configure a Custom Domain for Your Web App**

         To use your custom domain for linking to your web app, use the |R53| service to configure DNS
         routing.

         For a web app hosted in a single location, see `Routing Traffic to a Website that Is Hosted in
         an Amazon S3 Bucket <http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/RoutingToS3Bucket.html>`_.

         For a web app distributed through a global CDN, see `Routing Traffic to an Amazon CloudFront
         Web Distribution by Using Your Domain Name <http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-to-cloud-fron-distribution.html>`_






