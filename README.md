# Sending-Object-From-One-Activity-To-Another-
All of us have used intents to send and retrieve data from one activity to another.But, most of the time i found people Got Stuck How to send ArrayList of bean/pojo/model class from one Activity to another.Here is the way how you can achieve it
There are 2 ways to do it.
1. Serializable
2. Parcelable

 why to use Parcelable over Serializable
  1. Parcelable is well documented in the Android SDK; serialization on the other hand is available in Java.
     It is for this very reason that Android developers prefer Parcelable over the Serialization technique.
 
  2. In Parcelable, developers write custom code for marshaling and unmarshaling so it creates less garbage objects in comparison to      Serialization.
     The performance of Parcelable over Serialization dramatically improves (around two times faster),
     because of this custom implementation.
                                           Serialization is a marker interface, which implies the
     user cannot marshal the data according to their requirements.In Serialization, a marshaling operation is performed
     on a Java Virtual Machine (JVM) using the Java reflection API.This helps identify the Java objects member and
     behavior, but also ends up creating a lot of garbage objects.Due to this, the Serialization process is slow
     in comparison to Parcelable.
