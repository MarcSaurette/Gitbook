# Java 8

## Installing Java 8 on your machine

{% hint style="info" %}
Note:   
This tutorial is made for Linux users because they are the most likely to not have the correct version of Java pre-installed. If you are not a Linux user but are still facing issues and/or are uncomfortable using the Command Line/Terminal please [ask for help](../about.md#contact-us).
{% endhint %}

Open the terminal and check to see which version of Java is installed:

```
$ java -version
```

If the resulting output looks like this:  
`openjdk version "1.8.0_171"`  
  
Then the correct version of Java is installed and you do not need to make additional changes. If you see this output, but are still facing issues, go [here](../about.md#contact-us).

{% hint style="warning" %}
In the rare case that Java is not currently installed on your machine, you will see the following output:   
`Command 'java' not found`

You will need to install OpenJDK:  
`$ sudo apt install default-jre`
{% endhint %}

Install Java 8 by executing the following command:

```
$ sudo apt install openjdk-8-jdk
```

Check to see if the Java 8 was installed correctly:

```text
$ java -version
```

The resulting should look like this:  
`openjdk version "1.8.0_171"`

You now have Java 8 installed and running.

