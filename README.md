

# Awesome Cold Showers

It's great when people get excited about things, but sometimes they get a little _too_ excited. This an awesome (rigorous and respectful) and curated (I read every suggestion and make judgement calls) list of cold showers on overhyped topics. This does **not** mean the enthusiasm is bad or wrong: we're just reminding people to stay grounded. Feel free to submit your favorites!

####  [Verification Techniques](https://web.archive.org/web/20170214231046/https://www.cypherpunks.to/~peter/04_verif_techniques.pdf) (PDF)

* **Hype:** "Formal Verification is a great way to write software. We should prove all of our code correct."

* **Shower:** Extensive literature review showing that formal methods are hard to learn, extremely expensive to apply, and often miss critical bugs.

* **Caveats:** Written in 2000 and doesn't cover modern tools/techniques, such as TLA+ or dependent typing.

* **Notes:** Part of [Peter Gutmann](https://www.cs.auckland.ac.nz/~pgut001/)'s thesis, "The Design and Verification of a Cryptographic Security Architecture". The whole thesis can be found [here](https://archive.org/details/springer_10.1007-b97264/mode/2up).

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

* **Caveats:** Raw data you have to interpret yourself. ~~Does not provide a complete dump of the raw data for your own analysis.~~ Raw data can now be found [here](http://tfb-logs.techempower.com/)

* **Notes:** [Continually updating](https://tfb-status.techempower.com/) with new benchmarks. All implementations are public and you can improve them with a PR. 

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

#### [Fixing Faults in C and Java Source Code: Abbreviated vs. Full-word Identifier Names](http://www2.unibas.it/gscanniello/Giuseppe_Scanniello%40unibas/Home_files/TOSEM.pdf) (PDF)

* **Hype:** "Identifiers should be self-documenting! Use full names, not abbreviations." 

* **Shower:** Researchers had programmers fix bugs in a codebase, either with all of the identifiers were abbreviated, or where all of the identifiers were full-words. They found no difference in time taken or quality of debugging.

* **Caveats:** Only applies to fixing bugs. Otherwise watertight. This is honestly one of the most rigorous and comprehensive papers I've ever read. 

* **Notes:** Includes ethnography on how programmers debug abbreviated code. Link is to the author preprint. 

#### [An Eye Tracking Study on camelCase and under_score Identifier Styles (PDF)](http://www.cs.kent.edu/~jmaletic/papers/ICPC2010-CamelCaseUnderScoreClouds.pdf)

* **Hype:** camelCase is easier to read than under_score. So it is a best practice to
use camelCase in variable names, function names, and other identifiers.

* **Shower:** Several research papers have been done. But when eye-tracking software was
used to test the claim, two conclusions emerged: (1) developers are equally accurate
regardless of style, but (2) the under_score style can be processed faster and easier.

* **Caveats:** The study's sample size was small (15 people), and "Subjects were
historically trained mostly in the underscore identifier style and were all programmers."
In the study, subjects were presented terms in isolation (not in blocks of code). Thus,
as the study notes, there could be variance due to context. 

* **Notes:** "The interaction of Experience with Style indicates that novices benefit
twice as much with respect to time, with the underscore style.
"This paper purports to remedy difficulties in an earlier paper entitled
[To CamelCase or Under_score](http://citeseerx.ist.psu.edu/viewdoc/download;jsessionid=BD104CB69764CBBB36249528028E19B7?doi=10.1.1.158.9499&rep=rep1&type=pdf),
which concluded that with training, camelCase is more accurately processed. Finally, neither
paper seems to have analyzed whether native language comes into play (e.g. whether it is
easier for non-native English speakers to understand camelCase versus under_score).


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

#### [Scaling SQLite to 4M QPS on a Single Server](https://blog.expensify.com/2018/01/08/scaling-sqlite-to-4m-qps-on-a-single-server/)

* **Hype:** "Scaling out is better than scaling up. Cloud is more scalable than bare metal."

* **Shower:** Expensify found that running a single bare-metal server was both faster and cheaper than using a x1e.32xlarge EC2 instance. By using one server, they could avoid sharding their data.

* **Caveats:** Does not cover if scaling out bare metal has the same advantages over scaling out EC2 (assuming you can afford sharding). Can't really compare how much cheaper the bare metal is because they don't list the cost. I'm guessing their servers are 100k each? No basis for that guess though.

#### [Understanding Real-World Concurrency Bugs in Go (PDF)](https://songlh.github.io/paper/go-study.pdf)

* **Hype:** Compared to other languages, Go's concurrency system of goroutines and channels is easier to understand, easier to use, and is less prone to bugs and memory leaks.

* **Shower:** According to an empirical study by Tu, _et al_, there are plenty of concurrency-related bugs related to the difficulty in understanding and following the concurrency features and patterns provided by Go.

* **Caveats:** This study is specific to Go. Though other languages provide similar facilities, they are not covered in this article. Also, the types of bugs seen with channels and shared memory are different. Channels lead to more blocking bugs (deadlocks, dangling channels) while shared-memory lead to more nonblocking bugs (race conditions, dirty reads).

* **Notes:** "We studied six popular Go software including Docker, Kubernetes, and gRPC. We analyzed 171 concurrency bugs in total, with more than half of them caused by non-traditional, Go-specific problems"

## Plug

You can find my general ravings on my [website](https://hillelwayne.com) or [twitter](https://twitter.com/Hillelogram). 
