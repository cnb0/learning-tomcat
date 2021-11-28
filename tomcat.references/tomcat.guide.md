1. Getting Started with Tomcat
           
            Installing Tomcat
            Installing Tomcat on Linux
            Installing Tomcat from an Apache multiplatform binary release
            Installing Tomcat from this book's Linux RPM packages
            Installing Tomcat from the JPackage.org Linux RPM packages
            Installing Tomcat on Solaris
            Installing Tomcat on Windows
            Installing Tomcat on Mac OS X
            Installing Tomcat on FreeBSD
            Starting, Stopping, and Restarting Tomcat
            Starting Up and Shutting Down
            Environment variables
            Starting and stopping: The general case
            Starting and stopping on Linux
            Starting and stopping on Solaris
            Starting and stopping on Windows
            Starting and stopping on Mac OS X
            Starting and stopping on FreeBSD
            Common Errors
            Restarting Tomcat
            The general case
            Restarting Tomcat on Linux
            Restarting Tomcat on Solaris
            Restarting the Tomcat Windows Service
            Restarting Tomcat on Mac OS X
            Restarting Tomcat on FreeBSD
            Automatic Startup
            Automatic Startup on Linux
            Automatic Startup on Solaris
            Automatic Startup on Windows
            Automatic Startup on Mac OS X
            Automatic Startup on FreeBSD
            Testing Your Tomcat Installation
            Where Did Tomcat Come From?
            
2. Configuring Tomcat
            
            A Word About Using the Apache Web Server
            Relocating the Web Applications Directory
            Changing the Port Number from 8080
            Relaying Port 80 TCP Connections to Port 8080
            Running Tomcat on Port 80 via a Service Wrapper
            Common Errors
            Java VM Configuration
            Changing the JSP Compiler
            Managing Realms, Roles, and Users
            Realms
            UserDatabaseRealm
            JDBCRealm
            JNDIRealm
            JAASRealm
            Container-Managed Security
            Basic authentication
            Digest authentication
            Form authentication
            Client-cert authentication
            Single Sign-on
            Controlling Sessions
            Session Persistence
            StandardManager
            PersistentManager
            Using FileStore for storing sessions
            Using JDBCStore for storing sessions
            Accessing JNDI and JDBC Resources
            JDBC DataSources
            Other JNDI Resources
            Servlet Auto-Reloading
            Customized User Directories
            Tomcat Example Applications
            Common Gateway Interface (CGI)
            The Tomcat Admin Webapp
            
3. Deploying Servlet and JSP Web Applications in Tomcat
            
            Hosts
            The Host Manager Webapp
            Layout of a Web Application
            Deploying Servlets and JavaServer Pages
            Deploying an Unpacked Webapp Directory
            server.xml Context Deployment
            Context XML Fragment File Deployment
            Deploying a WAR File
            server.xml Context Deployment
            Context XML Fragment File Deployment
            Hot Deployment
            Working with WAR Files
            The Manager Webapp
            Automation with Apache Ant
            Building a JAR/WAR
            Deployment via Ant
            Copying the WAR file or webapp directory
            Accessing the Manager webapp
            The Tomcat standalone deployer
            The scp Ant Task
            Common Errors
            XML in property files
            FileNotFoundExceptions
            Symbolic Links
            
4. Tomcat Performance Tuning
            
            Measuring Web Server Performance
            Load-Testing Tools
            ab: The Apache benchmark tool
            Siege
            Apache Jakarta JMeter
            Web Server Performance Comparison
            Tomcat connectors and Apache httpd connector modules
            Benchmarked hardware and software configurations
            Benchmark procedure
            Benchmark results and            
            What else we could have benchmarked
            External Tuning
            JVM Performance
            Operating System Performance
            Internal Tuning
            Disabling DNS Lookups
            Adjusting the Number of Threads
            Speeding Up JSPs
            Precompiling JSPs by requesting them
            Precompiling JSPs at webapp start time
            Precompiling JSPs at build time using JspC
            Capacity Planning
            Anecdotal Capacity Planning
            Enterprise Capacity Planning
            Capacity Planning on Tomcat
            Additional Resources
            
5. Integration with the Apache Web Server
            
            The Pros and Cons of Integration
            Running Tomcat Standalone
            It's easier to set up
            No web server connector module to worry about
            Tomcat standalone is faster than Apache httpd proxying requests to Tomcat
            Potential for better security
            Ease of migration
            Ease of upgrades
            Tomcat has less supporting software
            Fewer people who know Tomcat's web server
            Fewer web server features
            Running Tomcat with Apache httpd
            Tomcat's web server is faster than Apache httpd
            More support software
            Faster startup and shutdown times
            More difficult to set up
            Tomcat dynamic content slowdown
            Potential for additional security holes
            More complicated upgrades
            Installing Apache httpd
            Apache Integration with Tomcat
            Sharing the Load Using Separate Port Numbers
            Apache httpd is oblivious to Tomcat security
            Twice the web servers to tune, maintain, and secure
            Awkward user experience and splintered logging
            Troublesome double authentication
            Proxying from Apache httpd to Tomcat
            Setting Up Apache httpd
            Setting Up Tomcat
            Verify That Proxying Works
            Disadvantages
            Apache httpd slows Tomcat's response time
            Twice the web servers to tune, maintain, and secure
            Troublesome dual authentication
            Proxying from Tomcat to Apache httpd
            Using the mod_jk Connector
            Using binary releases
            Compiling mod_jk
            Starting up the integrated servers
            workers.properties
            Tomcat Serving HTTP over the APR Connector
            Installing APR
            Using binary releases
            Compiling and installing APR
            Building and Installing the APR Connector
            Configuring Tomcat to Use the APR Connector

6. Tomcat Security
                        
            Securing the System
            Operating System Security Forums
            Configuring Your Network
            Multiple Server Security Models
            Using the SecurityManager
            Granting File Permissions
            Setting Up a Tomcat chroot Jail
            Setting Up a chroot Jail
            Using a Non-Root User in the chroot Jail
            Filtering Bad User Input
            Vulnerabilities
            Cross site scripting
            HTML injection
            SQL injection
            Command injection
            HTTP Request Filtering
            Installing the BadInputValve
            Installing the BadInputFilter
            See also
            Securing Tomcat with SSL
            Generating a Self-Signed Server Certificate
            Requesting and Installing a Commercial Certificate
            Setting Up an SSL Connector for Tomcat
            Configuring the JIO connector for SSL
            Configuring the APR connector for SSL
            Configuring the NIO connector for SSL
            Client Certificates


7. Configuration
            
            server.xml
            Server
            Service
            Executor
            Connector
            Engine
            Host
            Virtual hosting
            Alias
            Context
            Realm
            GlobalNamingResources
            Environment
            Resource
            ResourceEnvRef
            WatchedResource
            Listener
            Loader
            Manager
            Stores
            Resources
            Valve
            Controlling access logs with an access log valve
            RemoteHostValve and RemoteAddrValve
            Limiting request concurrency with SemaphoreValve
            Transaction
            Cluster
            Channel
            Membership
            Sender
            Transport
            Receiver
            Interceptor
            Member
            Deployer
            ClusterListener
            Migrating from Older Versions of Tomcat
            Migrating from 4.1 to 5.0
            Migrating from 5.0 to 5.5
            Migrating from 5.5 to 6.0
            web.xml
            web-app
            icon, display-name, and description
            distributable
            context-param
            filter and filter-mapping
            listener
            servlet
            servlet-mapping
            session-config
            mime-mapping
            welcome-file-list
            error-page
            jsp-config and taglib
            resource-env-ref
            resource-ref
            See also
            security-constraint
            See also
            login-config
            See also
            security-role
            env-entry
            See also
            ejb-ref and ejb-local-ref
            service-ref
            message-destination-ref
            message-destination
            locale-encoding-mapping-list
            tomcat-users.xml
            catalina.policy
            catalina.properties
            context.xml
            
8. Debugging and Troubleshooting
            
            Reading Logfiles
            Hunting for Errors
            URLs and the HTTP Conversation
            HTTP Requests
            Response Codes and Headers
            Interacting with HTTP
            Debugging with RequestDumperValve
            When Tomcat Won't Shut Down
            
9. Building Tomcat from Source
            
            Installing Apache Ant
            Obtaining the Source
            Downloading Source Code
            Obtaining Source Code from Apache's Subversion Repository
            Downloading Support Libraries
            Building Tomcat
            
10. Tomcat Clustering
            
            Clustering Terms
            The Communication Sequence of an HTTP Request
            DNS Request Distribution
            TCP NAT Request Distribution
            mod_proxy Load Balancing and Failover
            Distributed Java Servlet Containers
            Servlet sessions
            Session affinity
            Replicated sessions
            Tomcat 6 Clustering Implementation
            Features
            Configuring and Testing IP Multicast
            Configuring All-to-All Replication
            Testing Session Replication
            Configuring Static Membership
            Configuring Primary/Backup Replication
            JDBC Request Distribution and Failover
            
            
11. Final Words
            
            Supplemental Resources
            Online Documentation That Shipped with Tomcat
            The Apache Tomcat Web Documentation
            The Apache Tomcat Mailing List Archives
            Web Sites Related to This Book
            Third-Party Web Sites About Tomcat
            The #tomcat IRC Channel
            The Apache Tomcat Mailing Lists
            Community
            
A. Installing Java
            
            Choosing a Java JDK
            Working Around Older GCJ and Kaffe JVMs
            Sun Microsystems Java SE JDK
            IBM J9 JDK
            BEA JRockit JDK
            Apple Java SE JDK
            Excelsior JET
            Apache Harmony JDK
            
B. jbchroot.c
            
            C. BadInputValve.java
            D. BadInputFilter.java
            E. RPM Package Files