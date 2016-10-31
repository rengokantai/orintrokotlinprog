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
##Part 3: The Basics of Kotlin
###1 Declaring Variables in Kotlin
```
var a:Int
var b =""  //implictly
val c ="immutable"
```
###2 Working with Basic Types in Kotlin
Byte, Long, Float, Double Ex:
```
10L
100F
0x0F
0xb01   //binary
```
No explicit conversion in kotlin.
```
val myInt=10
val in:Long = myInt.toLong()
```
####04:40 multi line string
```
val l = """ line """
```
####05:20 string interpo
```
var a=1
var b=" a is $a"
var b=" a is ${a.length}"
```
