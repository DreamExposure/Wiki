DreamExposure Wiki
Plugins Novalib Developer Api Implentation
Discard
Save Changes

# Implementing NovaLib in Your Plugins

​

​

Implementing NovaLib is super simple! Just a quick dependency added into your project and you can start using NovaLib's robust API.

​

Everything that is accessible in the API when programming against it will be available in runtime.

​

Javadocs can be found here: https://docs.dreamexposure.org/plugins/novalib

​

## With Maven

Add this to your project's pom.xml, replacing “VERSION” with the target version of NovaLib. 

​

​

```xml

<repositories>

  <repository>

    <id>nova-public</id>

    <url>http://repo.novafox161.com/repository/nova-public/</url>

  </repository>

  ...

</repositories>

 

<dependencies>

  <dependency>

    <groupId>org.dreamexposure.novalib</groupId>

    <artifactId>API</artifactId>

    <version>VERSION</version>

    <scope>provided</scope>

    <type>jar</type>

  </dependency>

  ...

</dependencies>

```

​

## With Gradle

Add this to your project's build.gradle file, replacing “VERSION” with the target version. 

​

​

```groovy

  repositories {

    ...

    maven { url 'http://repo.novafox161.com/repository/nova-public/' }

  }

  

  dependencies {

    implementation 'org.dreamexposure.novalib:API:VERSION'

  }

```

​

## Without a Dependency Manager

irst, you will need to download the latest “NovaLib-API.jar” from the NovaLib Jenkins Job: https://jenkins.dreamexposure.org/job/NovaLib

​

Then just manually import the .jar file as a library for your project in whatever way your IDE supports. Instructions for some IDEs listed below. 

​

### IntelliJ IDEA

- Open up your project and wait until it finishes loading.

- Navigate to the “File > Project Structure” popup window.

- Select “Project Settings > Libraries”

- Click the “Plus” icon and select “Java”

- Navigate to the newly downloaded .jar and select “OK”

- You're all set! You can now use NovaLib in your plugin.

​

### Eclipse 

**Instructions coming soon**

​

​

# Conclusion

​

​

**Make sure to add “NovaLib” into your plugin's plugin.yml as a depend!!!**

​

That's all you need to do! You can now use NovaLib's API and library inside your plugin!

​

​

Powered by Wiki.js.

    Home
    Return to top