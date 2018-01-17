

# Awesome Cold Showers

It's great when people get excited about things, but sometimes they get a little _too_ excited. This an awesome (rigorous and respectful) and curated (I read every suggestion and make judgement calls) list of cold showers on overhyped topics. This does **not** mean the enthusiasm is bad or wrong: we're just reminding people to stay grounded. Feel free to submit your favorites!

####  [Verification Techniques](http://www.cypherpunks.to/~peter/04_verif_techniques.pdf) (PDF)

* **Hype:** "Formal Verification is a great way to write software. We should prove all of our code correct."

* **Shower:** Extensive literature review showing that formal methods are hard to learn, extremely expensive to apply, and often miss critical bugs.

* **Caveats:** Written in 2000 and doesn't cover modern tools/techniques, such as TLA+ or dependent typing.

* **Notes:** Part of [Peter Gutmann](https://www.cs.auckland.ac.nz/~pgut001/)'s thesis, "The Design and Verification of a Cryptographic Security Architecture".

#### [Static vs Dynamic Typing: a literature review](https://danluu.com/empirical-pl/)

* **Hype:** "Static Typing reduces bugs."

* **Shower:** A review of all the available literature (up to 2014), showing that the solid research is inconclusive, while the conclusive research had methodological issues.

* **Caveats:** Does not cover other possible benefits of static typing, like documentation. Does not address research on gradual type systems, like mypy or Typescript.

#### [Scalability! but at what COST?](http://www.frankmcsherry.org/graph/scalability/cost/2015/01/15/COST.html)

* **Hype:** "We need big data systems to handle big data."

* **Shower:** Benchmarking cutting-edge graph-processing algorithms running on 128-core clusters against a single-threaded 2014 Macbook Pro. The laptop consistently wins, sometimes by an order of magnitude.

* **Caveats:** McSherry is really good at optimizing his algorithms and has skills the average data scientist does not. Big data systems might be better if you have ad-hoc queries and don't want to take the time to optimize them.

* **Notes:** "If you are going to use a big data system for yourself, see if it is faster than your laptop. If you are going to build a big data system for others, see that it is faster than my laptop."

#### [Web Framework Benchmarks](https://www.techempower.com/benchmarks/)

* **Hype:** Anything about performance or scalability of various languages/web frameworks/databases.

* **Shower:** Actual hard data of various combinations of solutions under various tasks.

* **Caveats:** Raw data you have to interpret yourself. Does not provide a complete dump of the raw data for your own analysis.

* **Notes:** Updates with new benchmarks and frameworks once a year. All implementations are public and you can improve them with a PR. 

#### [Agile Methods: The Good, the Hype and the Ugly](https://www.youtube.com/watch?v=ffkIQrq-m34) (Video)

* **Hype:** "We should develop software using Agile."

* **Shower:** Review of all the different styles of Agile and how some of the practices (particularly replacing requirements with user stories and the lack of proper specification) are harmful in the long run.

* **Caveats:** While Meyer calls out some problems, overall he's very positive about Agile and recommends it as a good (but imperfect) methodology.

* **Notes:** Starts at [3:30](https://youtu.be/ffkIQrq-m34?t=3m30s). There's a [followup video](https://www.youtube.com/watch?v=Q_9k6ym5BZU) where he answers audience questions. 

#### [An Empirical Study on the Correctness of Formally Verified Systems](https://homes.cs.washington.edu/~pfonseca/papers/eurosys2017-dsbugs.pdf) (PDF)

* **Hype:** "If I formally verify my code, I don't need to test it!"

* **Shower:** Researchers looked at three formally verified systems, and found critical correctness bugs in all three. The bugs were from "a wide range of mismatched assumptions" and caused servers to crash or produce wrong data.

* **Caveats:** Most bugs were at the system boundaries; none were found in the implemented protocols. Formally verified systems, while not perfect, were considerably less buggy than unverified systems.

* **Notes:**  Systems were verified with Coq and Z3. Further discussion at [The Morning Paper](https://blog.acolyer.org/2017/05/29/an-empirical-study-on-the-correctness-of-formally-verified-distributed-systems/).

#### [Fixing Faults in C and Java Source Code: Abbreviated vs. Full-word Identiﬁer Names](http://www2.unibas.it/gscanniello/Giuseppe_Scanniello%40unibas/Home_files/TOSEM.pdf) (PDF)

* **Hype:** "Identifiers should be self-documenting! Use full names, not abbreviations." 

* **Shower:** Researchers had programmers fix bugs in a codebase, either with all of the identifiers were abbreviated, or where all of the identifiers were full-words. They found no difference in time taken or quality of debugging.

* **Caveats:** Only applies to fixing bugs. Otherwise watertight. This is honestly one of the most rigorous and comprehensive papers I've ever read. 

* **Notes:** Includes ethnography on how programmers debug abbreviated code. Link is to the author preprint. 

#### [Microservices - Please, don't](http://basho.com/posts/technical/microservices-please-dont/)

* **Hype:** "Microservices! Microservices!"

* **Shower:** Presents five fallacies of "why microservices solve problems monoliths have" and shows how either monoliths don't actually have those problems or that microservices make the problem even worse. 

* **Caveats:** Abstract arguments and experience, no case studies or examples.

#### [VM Warmup Blows Hot and Cold](https://arxiv.org/abs/1602.00602)

* **Hype**: Your favourite programming language has been updated. The new
  version makes impressive performance improvement claims.

* **Shower**: Benchmarking modern programming languages under near-ideal
  circumstances, just for longer than before, suggests that we have not been
  benchmarking language implementations as accurately as we might wish. Many
  benchmarks slow down over time. Some never stabilise. Many benchmarking
  experiments will not be repeatable due to non-determinism. Warmup time is
  important, but is usually either ignored, or reported inaccurately.

* **Caveats**: Only evaluates the x86_64 architecture, and for only two
  operating systems (Linux and OpenBSD). Experiment conducted in 2017 (prior to
  meltdown patching). Evaluates mainly JITted language implementations
  (although C benchmarks were included).

 * **Notes**: The experiment and the benchmark runner are published under an
   open source license. [Start here](https://github.com/softdevteam/warmup_experiment).

## Plug

You can find my general ravings on my [website](https://hillelwayne.com) or [twitter](https://twitter.com/Hillelogram). 
