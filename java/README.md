# HelloTF for Java

To start with Java, you need to first to setup a maven project and add following dependency in your pom.xml.

```
<dependency>
  
  <groupId>org.tensorflow</groupId>
  
  <artifactId>tensorflow</artifactId>
  
  <version>1.7.0</version>

</dependency>
```

This is enumuration a enumuration of two library 
 - libtensorflow
 - libtensorflow_jni
 
This wrap TensorFlow C++ library and JNI connector to access it through java programs. 

Additionaly, you can add following dependency to support GPU accelration by default it work on CPU powers.

```
<dependency>
  
  <groupId>org.tensorflow</groupId>

  <artifactId>libtensorflow_jni_gpu</artifactId>
  
  <version>1.7.0</version>

</dependency>
```

Now you are all set to use TensorFlow features on Java. 

You can use following test program to check the environment.

[HelloTF.java](java/src/main/java/HelloTF.java)

This is basically creating an Operation Graph with a Const and assigning value as current version. For fetching it you need to run it inside a session.
