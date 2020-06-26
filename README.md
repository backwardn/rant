# NOTICE: Repisitory Archived

**As of 26 June, 2020, this repository is now archived.**

Due to a variety of reasons, I have decided to formally end maintenance of the Rant repository.
It will remain permanently available at this location in a read-only state.

Since Rant's inception in 2013, I have learned quite a lot about what it means to write good software, and readily acknowledge that the language and runtime are fundamentally poorly-designed, poorly-documented, and poorly-supported. I have listened carefully to all of your comments (especially the criticism) and I cannot, in good conscience, continue to contribute to this project in its current state.

This is not, however, the end of Rant itself. My goal has always been to deliver a product that I am confident will be a worthy contribution to the toolsets of creatives and developers everywhere, and I will continue to pursue that goal. My plan for the new Rant 4 is to completely reimagine the language from the ground up using the Rust programming language to develop a new compiler and runtime vastly superior in both performance and cross-platform support.

When I am ready to share more information regarding the development of Rant 4, I will post updates on my Twitter ([@TheBerkin](https://twitter.com/TheBerkin)). 

Thank you to everyone who has supported and contributed to Rant over the years. I hope to far exceed your expectations with the next release.

***
Original readme:

<p align="center">
<img src="http://i.imgur.com/Vx7LyRP.png" alt="Rant logo" height="225px" width="225px"></img>
</p>
<br/>

**Rant** is an all-purpose procedural text engine
that is most simply described as the opposite of Regex.
It has been refined to include a dizzying array of features for handling everything from
the most basic of string generation tasks to advanced dialogue generation,
code templating, automatic formatting, and more.

The goal of the project is to enable developers of all kinds
to automate repetitive writing tasks with a high degree of creative freedom.
<p align="center">
<a href="https://ci.appveyor.com/project/TheBerkin/rant/branch/master/artifacts">
    <img src="https://ci.appveyor.com/api/projects/status/2vn0imlns20n739a/branch/master?svg=true&passingText=Master%20Build%20Passing&pendingText=Master%20Build%20Pending&failingText=Master%20Build%20Failing" alt="Build status" />
  </a>
  <a href="https://ci.appveyor.com/project/TheBerkin/rant/branch/dev/artifacts">
    <img src="https://ci.appveyor.com/api/projects/status/2vn0imlns20n739a/branch/dev?svg=true&passingText=Dev%20Build%20Passing&pendingText=Dev%20Build%20Pending&failingText=Dev%20Build%20Is%20Kill" alt="Build status" />
  </a>
  <img src="https://img.shields.io/nuget/dt/Rant.svg" title="NuGet Downloads"/>
  <br/>
  <b>Join us on the official <a href="https://discord.gg/5n7bnAD">Discord server</a>!</b>
</p>

## Features

* Recursive, weighted branching with several selection modes
* Queryable dictionaries
* Automatic capitalization, rhyming, English indefinite articles, and multi-lingual number verbalization
* Print to multiple separate outputs
* Probability modifiers for pattern elements
* Loops, conditional statements, and subroutines
* Fully-functional object model
* Import/Export resources easily with the .rantpkg format
* Compatible with Unity 2017
* *And much, much, much more...*

## Examples

**Liven up a narrative with a few simple queries.**
```
<name-male> likes to <verb-transitive> <noun.pl> with <pro.dposs-male> pet <noun-animal> on <noun.pl  -dayofweek>.
```
```
Alick likes to mount shuttlecocks with his pet bat on Mondays.
```

---

**Count to ten and spell it out.**
```
[case:sentence][numfmt:verbal][rs:10;\s]{[rn].}
```
```
One. Two. Three. Four. Five. Six. Seven. Eight. Nine. Ten.
```

---

**Write a poem**
```
[rhyme:perfect]
The <noun(1)::&a> <verb.ed(1)-transitive::&a> the <adj::&a> <noun(1)::&a>.
```
```
The bread fed the red head.
```
```
The drug dug the smug plug.
```

---


## NuGet
Rant is also available as a [NuGet package](https://www.nuget.org/packages/Rant/).
Enter this command in your package manager,
and the latest version of Rant will automagically get installed in your project:

```
PM> Install-Package Rant
```

Or if development builds are your thing:

```
PM> Install-Package Rant -Pre
```

## License
Rant is provided under [The MIT License](https://github.com/TheBerkin/Rant/blob/master/LICENSE).

## Improve Rant
If there is something you want fixed, added, or changed, feel free to submit an issue/pull request; I will try to get back to you within a day. If you would like to translate Rant into your native language, simply write a .lang file for it [like this one here](https://github.com/TheBerkin/rant/blob/master/Rant/Localization/en-US.lang).

See [CONTRIBUTING.md](CONTRIBUTING.md) for a full guide on how you can help.

## Rant Resources

* [Rant Homepage](http://berkin.me/rant)
* [Rant Documentation](http://berkin.me/rant/docs)
* [Rant Demos](https://github.com/TheBerkin/Rant.Demos)
* [Rant Standard Dictionary](https://github.com/TheBerkin/Rantionary)
* [Online Pattern Tester](http://lett.at/rantbox/)
