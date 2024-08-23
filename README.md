# Hi 👋

```Scala
@main
def welcome(): Unit = {
  val me = SoftwareEngineer(
    name = "Timo Erdelt",
    role = "Full Stack Software Engineer",
    company = "Unit 214 GmbH",
    languages = Seq("de-DE", "en-US", "es-ES"),
    technologies = Seq("Scala", "TypeScript", "React", "Rust", "Go")
  )
  me.sayHi()
  me.introduce()
  me.sayGoodbye()
}

class SoftwareEngineer(name: String,
                       role: String,
                       company: String,
                       languages: Seq[String],
                       technologies: Seq[String]) {
  def sayHi(): Unit =
    println(s"Hi there, thank you for dropping by!")

  def introduce(): Unit = {
    println(s"My name is $name.")
    println(s"I'm a $role @ $company.")
    println(s"I speak the following languages: ${languages.mkString(", ")}.")
    println(s"My favorite technologies include: ${technologies.mkString(", ")}.")
  }

  def sayGoodbye(): Unit = {
    println(s"Feel free to connect or explore some of my repositories. Until next time!")
  }
}
```
