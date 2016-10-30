# orintrokotlinprog
##Part 2: A Primer on Kotlin
###4 The Structure of a Kotlin Application
Main.kt
```
fun main(args:Array<String>){
  println("")
}
```

use java to compile
```
java -cp .:/usr/local/Ke/kotlin/1.0.4/libexec/lib/kotlin-runtime.jar me.yd.MainKt
```
because
```
kotlinc Main.kt
```
will generate
```
/.idea
/me   //folder
MainKt.class
```

####09:21 create jar
```
kotlinc Main.kt -d hello.jar
```
make a kotlin-generated jar include runtime
```
kotlinc Main.kt -inclide-runtime -d hello.jar
```
then we can run using java directly
```
java -jar hello.jar
```
