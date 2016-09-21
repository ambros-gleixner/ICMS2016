# ICMS 2016 Session: Mathematical Optimization

ICMS 2016: [Home](http://icms2016.zib.de), [Sessions](http://icms2016.zib.de/sessions.html)

> Deadline extension: **NOVEMBER 15, 2016** for submission to our [Special Issue of Optimization Methods & Software](#call-for-papers-special-issue-of-optimization-methods-and-software) on *Mathematical Optimization Software*, see below.

## Organizers

* [Ambros Gleixner](http://www.zib.de/gleixner), Zuse Institute Berlin, Germany
* [Christian Kirches](http://www.iwr.uni-heidelberg.de/groups/optimus/people/kirches), IWR Heidelberg/TU Braunschweig, Germany
* [John Mitchell](http://www.rpi.edu/~mitchj), Rensselaer Polytechnic Institute, USA
* [Ted Ralphs](http://coral.ie.lehigh.edu/~ted), Lehigh University, USA

## Aim & Scope

One out of four mathematical software packages listed in the database swMATH.org is categorized under the search term optimization. This indicates the prominent role of computational research in the field of optimization, and vice versa. This session aims at spanning the broad range of mathematical optimization software from algorithms for continuous, convex optimization that exploit strong duality theory to solver software for nonconvex problem classes, including packages that support the modeling process.

Recent developments that deserve special, though not exclusive attention are the integrated handling of nonconvex constraints from discrete and continuous optimization, the exploitation of increasingly available parallel hardware architecture, and arithmetically exact methods that render optimization a tool for mathematical theory exploitation. The session shall provide a forum for discussing common and distinct challenges and future trends.

Possible topics include, but are not limited to:
* linear and nonlinear programming solvers,
* conic optimization and interior-point methods,
* mixed-integer optimization,
* algorithms for complementarity problems,
* (mixed-integer) optimal control,
* multi-objective and multi-level optimization,
* modeling languages and solver interfaces,
* testing and benchmarking of optimization software,
* software design,
* parallel algorithms,
* numerical stability,
* optimization over large data sets,
* applications of optimization software in practice,
* etc.

## Submission Guidelines & Publications

A **short abstract** will appear on the permanent conference web page (see below) as soon as accepted.
An **extended abstract** will appear in the [proceedings](http://dx.doi.org/10.1007/978-3-319-42432-3) and will be distributed during the meeting.
A **special issue** of the journal *Optimization Methods & Software* consisting of full papers will be organized immediately after the meeting.  See details [below](#call-for-papers-special-issue-of-optimization-methods-and-software).

> This session is now closed for new submissions, but note that submission to the special issue **does not require participation in ICMS 2016** and is open to all relevant contributions.


## Talks & Abstracts

### Monday, July 11, 16:00-17:40

#### Recent developments in Optimization Services (OS)

Authors: [Horand I. Gassmann](http://myweb.dal.ca/gassmann), Jun Ma, Kipp Martin, and Imre Polik

Optimization Services (OS) is an open-source project under COIN-OR and provides infrastructure for the solution of optimization problems over the internet. This includes a number of XML schemas for the transmission of problem instances, options and solutions as well as related information; and interfaces to a number of open-source and commercial solvers.  This talk presents recent developments, such as support for the description of matrices within the OSiL format, an interface to the open-source SDP solver CSDP, and schema elements to describe real-time data elements, problem modifications, disjunctions, and stochastic information.

#### CMPL (\<Coliop|Coi\> Mathematical Programming Language)

Authors: [Ted Ralphs](http://coral.ie.lehigh.edu/~ted) and [Mike Steglich](https://www.th-wildau.de/homepages/mike-steglich/ms-startseite.html)

Slides: [slides/steglich.pdf](slides/steglich.pdf)

CMPL is a system for mathematical programming and optimisation of linear optimisation problems using popular solvers such as CBC, GLPK, SCIP, Gurobi and CPLEX.  After an overview of the main functionality and the features of the language, CMPL's application programming interfaces for Python and Java (pyCMPL and jCMPL) will be presented. The next step will describe how CMPL, pyCMPL and jCMPL can be used with the CMPLServer; an XML-RPC-based web service for distributed and grid optimisation. The talk will finish with an overview of the main aspects of CMPL's integration with SolverStudio and it will be shown how CMPL and pyCMPL models can be solved within Excel and SolverStudio.

#### PySCIPOpt: Mathematical Programming in Python with the SCIP Optimization Suite

Authors: Stephen J Maher, [Matthias Miltenberger](http://www.zib.de/miltenberger), João Pedro Pedroso, Daniel Rehfeldt, Robert Schwarz, and Felipe Serrano

Slides: http://www.zib.de/miltenberger/ICMS_2016_PySCIPOpt.slides.html

When it comes to customized mathematical programming, SCIP is often the software of choice: Its plug-in based design provides a simple method of extension to handle a variety of specific problem classes and it moreover allows for ubiquitous mastery of the solving procedure and access to detailed processual information. Furthermore, SCIP has frequently distinguished itself as being state-of-the-art in academic discrete optimization.  However, with its source written in C, SCIP can prove challenging for inexperienced users wishing to implement hand-tailored extensions. This paper attempts to provide a remedy by introducing PySCIPOpt, a Python interface to SCIP that enables users to write new SCIP code entirely in Python. In this way, fast prototyping of new algorithmic ideas without the coding overhead of the C language is possible. We demonstrate how to intuitively model mixed-integer linear and quadratic optimization problems and moreover provide examples on how new Python plug-ins can be added to SCIP.

#### DSJM: A Software Toolkit for Direct Determination of Sparse Jacobian Matrices

Authors: [Shahadat Hossain](http://www.cs.uleth.ca/~hossain) and Ahamad Imtiaz Khan

We describe the architecture and implementation of DSJM, a software toolkit written in portable C++ that enables direct determination of sparse Jacobian matrices. Our design exploits the recently proposed unifying framework "pattern graph" and employs cache-friendly array-based sparse data structures. The pattern graph remains invariant for one-sided, two-sided, full column, and column-segments compression algorithms.
The DSJM implements a greedy partitioning algorithm after the sparse matrix has been preprocessed with ordering heuristics for efficiency. In our numerical testing on 20 large-scale test instances (see *Graph Models and their efficient implementation for sparse Jacobian matrix determination, Disc. Appl. Math. 161(2013):1747-1754*) we have found that DSJM consistently produced better timing and partitions compared with similar software.

#### SolverStudio and OpenSolver: Excel Tools for Bringing Advanced Optimisation to the Masses

Author: [Andrew Mason](http://www.esc.auckland.ac.nz/Mason)

OpenSolver (http://opensolver.org) is an open source Excel add-in that makes a variety of linear and non-linear optimisation solvers easily accessible to both the academic and wider Excel communities. OpenSolver has proven very popular, with download counts approaching the 180,000 mark. This presentation will briefly outline some of the new features of OpenSolver and present several case studies illustrating its use.
While Excel makes it easy to build optimisation models, these models can be difficult to scale and debug. SolverStudio, another free spreadsheet add-in for Excel, has been developed to better meet the needs of more advanced optimisation users. Unlike OpenSolver, SolverStudio (http://solverstudio.org) allows users to build their models using popular modelling languages such as PuLP, AMPL, GAMS, CMPL and Julia/JUMP. However, unlike other tools, SolverStudio removes the need to learn a new software environment and instead allows the user to develop, test and deploy their optimisation model all within Excel. This presentation will demonstrate SolverStudio and several example applications.


### Tuesday, July 12, 10:30-12:10

#### Parallel distributed-memory simplex for large-scale stochastic LP problems

Authors: Miles Lubin, [J. A. Julian Hall](http://www.maths.ed.ac.uk/hall), Cosmin G. Petra, and Mihai Anitescu

Although parallel efficiency using the revised simplex method has not been achieved for general large sparse LP problems, this talk will show how the particular structure of stochastic LP problems gives scope for efficient data parallelism.

Very large stochastic LP problems have been considered to be too big to solve with the simplex method, with decomposition approaches or, more recently, interior-point methods being preferred. However, these approaches do not provide optimal basic solutions which allow for the efficient hot-starts required, for example, in a branch-and-bound context when solving stochastic MIP problems.

Our approach exploits the dual block-angular structure of these problems inside the linear algebra of the revised simplex method in a manner suitable for high-performance distributed-memory clusters or supercomputers. While the focus is on stochastic LPs, the work is applicable to all problems with a dual block-angular structure. Our implementation is competitive in serial with highly efficient sparsity-exploiting simplex codes and achieves parallel efficiency when using up to 128 cores and runs up to 100 times faster than the leading open-source serial solver. Additionally, very large problems with hundreds of millions of variables have been successfully solved to optimality: possibly the largest LPs ever solved using the simplex method.

This is the largest-scale parallel sparsity-exploiting revised simplex implementation that has been developed to date and the first truly distributed solver. It is built on novel analysis of the linear algebra for dual block-angular LP problems when solved by using the revised simplex method and a novel parallel scheme for applying product-form updates.

#### Parallelization of the FICO Xpress Optimizer

Authors: [Timo Berthold](http://www.zib.de/berthold), James Farmer, Stefan Heinz, and Michael Perregaard

Slides: [slides/berthold.pdf](slides/berthold.pdf)

We will present some of the recent MIP advances in the FICO Xpress Optimizer, with an emphasis on its new parallelization concept. To achieve reasonable speedups from parallelization, a high workload of the available computational resources is a natural precondition. At the same time, reproducibility and reliability are key requirements for mathematical optimization software. Thus, parallel LP-based branch-and-bound algorithm are expected to be fully deterministic. The resulting synchronization latencies render the goal of a satisfying workload a challenge of its own. We address this challenge by following a partial information approach and separating the concepts of simultaneous tasks and independent threads from each other. Our computational results indicate that this leads to a much higher CPU workload and thereby to an improved scaling on modern high-performance CPUs. As an added value, the solution path that the Optimizer takes is not only deterministic in a fixed environment, but on top of that platform- and, to a certain extent, thread-independent.

#### A First Implementation of ParaXpress: Combining Internal and External Parallelization to Solve MIPs on Supercomputers

Authors: [Yuji Shinano](http://www.zib.de/members/shinano), Timo Berthold, and Stefan Heinz

The Ubiquity Generator (UG) is a general framework for the external parallelization of MIP solvers. It has been used to develop ParaSCIP, a distributed memory, massively parallel version of the open source solver SCIP, running on up to 80,000 cores.  In this paper, we present a first implementation of ParaXpress, a distributed memory parallelization of the powerful commercial MIP solver FICO Xpress. Besides sheer performance, an important difference between SCIP and Xpress is that Xpress provides an internal parallelization for shared memory systems.  When aiming for a best possible performance of ParaXpress on a supercomputer, the question arises how to balance the internal Xpress parallelization and the external parallelization by UG against each other.  We provide computational experiments to address this question and we show preliminary computational results for running a first version of ParaXpress on 6,144 cores in parallel.

#### pyADCG: A preliminary implementation of a new parallel solver for nonconvex MINLPs in Pyomo/Python

Authors: [Ivo Nowak](https://www.haw-hamburg.de/ti-mp/unser-department/beschaeftigte/name/ivo-nowak.html) and Norman Breitfeld

Slides: [slides/nowakbreitfeld.pdf](slides/nowakbreitfeld.pdf)

In this talk we present pyADCG, a preliminary implementation of a new parallel decomposition method for nonconvex MINLPs in Pyomo/Python. The new optimization method, called ADCG (Alternating Direction Column Generation), is not based on the branch-and-bound approach. The basic idea of ADCG is to restrict the objective value by a target constraint and to check via a column generation based globally convergent alternating direction method if the resulting MINLP is feasible or not.  Convergence is shown by using the fact that the duality gap of a general nonconvex projection problem is zero, see http://www.optimization-online.org/DB_HTML/2015/12/5233.html.  We discuss algorithmic variants and report first numerical results.

#### Advanced Computing & Optimization Infrastructure for Extremely Large-Scale Graphs on Post Peta-Scale Supercomputers

Author: [Katsuki Fujisawa](http://sdpa.imi.kyushu-u.ac.jp/~fujisawa)

In this talk, we present our ongoing research project. The objective of this project is to develop advanced computing and optimization infrastructures for extremely large-scale graphs on post peta-scale supercomputers. We explain our challenge to Graph 500 and Green Graph 500 benchmarks that are designed to measure the performance of a computer system for applications that require irregular memory and network access patterns. The 1st Graph500 list was released in November 2010. The Graph500 benchmark measures the performance of any supercomputer performing a BFS (Breadth-First Search) in terms of traversed edges per second (TEPS). In 2014 and 2015, our project team was a winner of the 8th,10th, and 11th Graph500 and the 3rd to 6th Green Graph500 benchmarks, respectively.

We also present our parallel implementation for large-scale SDP (SemiDefinite Programming) problem. The semidefinite programming (SDP) problem is a predominant problem in mathematical optimization. The primal-dual interior-point method (PDIPM) is one of the most powerful algorithms for solving SDP problems, and many research groups have employed it for developing software packages. We solved the largest SDP problem (which has over 2.33 million constraints), thereby creating a new world record. Our implementation also achieved 1.774 PFlops in double precision for large-scale Cholesky factorization using 2,720 CPUs and 4,080 GPUs on the TSUBAME 2.5 supercomputer.

### Tuesday, July 12, 14:20-16:00

#### High-Precision Quadratic Programming by Iterative Refinement

Authors: Ambros Gleixner, Sebastian Sager, and [Tobias Weber](https://www.math.uni-magdeburg.de/institute/imo/ag_sager/PEOPLE/Weber)

Quadratic programming (QP) problems are an important class of optimization problems arising in many applications. Usually it suffice to (and most QP solvers do) approximate the solution of the QP in floating-point arithmetic. However, it may be of interest to calculate solutions of higher precision. We present the extension of iterative refinement for linear programming to QP problems.

A sequence of similar QP problems with identical constraint and objective matrices is solved in floating-point arithmetics. These problems differ in the linear objective term, the right hand side of the constraints, and the bounds. Standard active set QP solvers should be used to solve them, preferably having hot (warm) start capabilities. Then, using exact arithmetic, the solution of each QP problem is used to improve the precision of the initial solution. It is also used to calculate a new refined QP problem for the next iteration. This procedure is repeated iteratively until the desired precision is reached.  We present first numerical results for convex QP instances using the qpOASES solver.

#### Efficient Validation of Basic Solutions via the Roundoff-Error-Free Factorization Framework

Authors: [Adolfo R. Escobedo](https://sites.google.com/site/adolfoescobedo1) and Erick Moreno-Centeno

The Roundoff-Error-Free (REF) LU and Cholesky factorizations, combined with the REF substitution algorithms, allow systems of linear equations to be solved without accruing roundoff errors and without excessive matrix entry growth, thereby permitting linear and mixed-integer programming problems to be solved exactly and efficiently. These REF computational tools aim to make significant advances to the field of optimization for two reasons: (1) solutions yielded by commercial mathematical programming solvers do not come with a certificate of validity; (2) in-use exact solvers implement exact validation subroutines that rely on rational arithmetic which, unlike the featured framework, is hampered by its repeated use of expensive greatest common divisor operations to bound matrix entry growth.

This work contains several computational tests showing that the REF framework solves systems of linear equations up to two orders of magnitude quicker than the exact rational arithmetic LU factorization method and requiring asymptotically half the memory. Moreover, we adapt Edmond’s integer-preserving Q-Matrix method to serve as a basic solution validation tool, and perform additional experiments that demonstrate that the REF factorization framework remains significantly superior in terms of memory requirements and computational effort.


#### On Solution Algorithms for Time-Dependent Quasi-Variational Inequalities with Gradient Constraints

Authors: [Rafael Arndt](TODO), Michael Hintermueller, and Carlos N. Rautenberg

Slides: [slides/arndt.pdf](slides/arndt.pdf)

We consider non-dissipative quasi-variational inequalities with pointwise constraints on the gradient of the state.  Such problems arise, for example, in the modeling of growing piles of cohesionless granular materials and water drainage on a given surface.  In these cases, the associated gradient constraint involves both a material-specific angle of repose and local properties of the concerned supporting structure.  Existence of a solution is shown and appropriate regularizations for numerical realization are adressed. For this type of non-convex problems, we derive solution algorithms in function space, considering two approaches: a variable splitting method, resulting in an alternating minimization scheme, and a semismooth Newton method.  Convergence results are shown in both cases.  Additionally we provide counter-examples to popular approaches when dealing with quasi-variational inequalities of this type. Numerical experiments of sandpile growth and of water drainage for certain topologies are presented.

#### Global error control for Optimal Control problems

Authors: [Andreas Meyer](https://typo.iwr.uni-heidelberg.de) and Andreas Potschka

For the numerical solution of large-scale ODE and DAE constrained optimal control problems (OCPs), direct transcription methods like Direct Multiple Shooting and Collo- cation have been established as the methods of choice. In these approaches, the infinite dimensional OCP is suitably discretized in order to obtain a finite dimensional Nonlinear Programming Problem. However, the discretization is often performed with no or at most local control of the discretization error. In this contribution we propose an error controlled adaptive mesh refinement strategy for a particular pseudospectral collocation method. Our error estimator is based on duality principles and Galerkin orthogonality, which are the ba- sis of computing elementwise discretization error contributions to the global discretization error. The equilibration of local error contributions in combination with detection of non- smoothness of solutions leads to efficient collocation meshes and a corresponding sequence of NLPs with increasing dimensionality. The proposed methods have been implemented in a software package. Finally, we give an outlook on a pseudospectral collocation approach for switched optimal control problems that leads to a sequence of mixed-integer NLPs.

#### Solving the Trust-Region Subproblem using Krylov subspace methods

Authors: [Felix Lenders](https://typo.iwr.uni-heidelberg.de) and Christian Kirches

Solving the Trust-Region Subproblem constitues an important ingredient in modern algorithms for nonlinear optimization problems. We present a method that builds on the successful GLTR algorithm (Gould et al 1999) in which expanding Krylov subspaces are iteratively assembled and a restricted version of the subproblem in these is solved. Particular attention is paid to the hard case and multiple invariant Krylov subspaces. We introduce an implementation of the method in C that employs a vector free reverse communication interface which allows to use adaptivity when solving functionspace problems and structure exploitation in lifted optimization problems as they commonly arise in optimal control.

### Tuesday, July 12, 16:20-18:00

#### SCIP-SDP: A Framework for Solving Mixed-Integer Semidefinite Programs

Authors: [Tristan Gally](http://www3.mathematik.tu-darmstadt.de/index.php?id=2575), Marc E. Pfetsch, and Stefan Ulbrich

Slides: [slides/gally.pdf](slides/gally.pdf)

Mixed-integer semidefinite programs arise in many applications and several problem-specific solution approaches have been studied recently. In this talk, we present a generic branch-and-bound framework for solving such problems.

We will first give a short overview of applications of mixed-integer semidefinite programming, including truss topology design, cardinality constrained least squares and minimum k-partitioning. Afterwards, we will investigate the strong duality of semidefinite relaxations arising in a branch-and-bound context. Furthermore, we will discuss strategies for enhancing the solution process of a branch-and-bound approach to mixed-integer semidefinite programming, including branching, dual fixing and heuristics. Finally, we will present numerical results demonstrating the applicability of the proposed framework and the success of the proposed techniques.

#### Improving BiqMac: stronger semidefinite relaxations for solving binary quadratic problems

Author: [Angelika Wiegele](http://wwwu.uni-klu.ac.at/anwiegel)

Max-cut is a classical NP-hard combinatorial optimization problem that has attracted the attention of many mathematicians and computer scientists during the past decades. The solver BiqMac is among the best performing solver for finding exact solutions of the Max-Cut problem. Any unconstrained binary quadratic problem can be transformed into a max-cut problem and thus can also be solved using BiqMac for instances of medium size.

The algorithm inside BiqMac is based on a relaxation of max-cut using semidefinite programming (SDP). It consists of a branch and bound setting, using a basic SDP bound strengthened by the so-called triangle inequalities to obtain high-quality upper bounds. To solve this SDP relaxation a dynamic version of the bundle method is implemented.

We now aim in improving BiqMac by finding even stronger bounds by considering exact subgraph constraints. These are constraints for classes of problems based on graphs for which the projection of the problem onto a subgraph shares the same structure as the original problem. Obviously, the max-cut problem has this property. Including these constraints immediately raises the question of solving the underlying relaxation. Again, we will use a bundle method, but will have to tailor it considering the new constraints.

A future project is to code the algorithm such that various parts will run in parallel leading to a vast speed-up of the solver. Furthermore, we want to widen the applicability of BiqMac by considering a transformation of linearly constrained binary quadratic problems into unconstrained ones by using ideas from exact penalty methods.

#### Software for cut generating functions in the Gomory-Johnson model and beyond

Authors: Chun Yu Hong, [Matthias Köppe](http://www.math.ucdavis.edu/~mkoeppe), and Yuan Zhou

I will present software (with C. Y. Hong and Y. Zhou), available at https://github.com/mkoeppe/infinite-group-relaxation-code, for investigations with cut generating functions in the Gomory-Johnson model and extensions, implemented in the computer algebra system SageMath.

#### PolySCIP - a solver for multi-criteria optimization problems

Authors: Ralf Borndörfer, [Sebastian Schenker](http://www.zib.de/members/schenker), Martin Skutella, and Timo Strunk

PolySCIP is a new solver for multi-criteria integer as well as multi-criteria linear programs handling an arbitrary number of objectives. It is available as an official part of the non-commercial constraint integer programming framework SCIP. It utilizes a lifted weight space approach to compute the set of supported extreme non-dominated (SEN) points and unbounded non-dominated rays, respectively. The algorithmic approach can be summarized as follows: At the beginning an arbitrary SEN point is computed (or it is determined that there is none) and a weight space polyhedron created. In every next iteration a vertex of the weight space polyhedron is selected whose entries yield a single-objective optimization problem via a combination of the original objectives. If the optimization of this single-objective problem leads to a new SEN point, the weight space polyhedron is updated. Otherwise another vertex of the weight space polyhedron is investigated. The algorithm finishes if all vertices of the weight space polyhedron have been investigated and no update steps of the polyhedron are necessary anymore. The file format of PolySCIP is based on the widely used MPS format and allows a simple generation of multi-criteria models via an algebraic modelling language.

#### Mixed Integer Nonlinear Programming for Minimization of Akaike's Information Criterion

Authors: [Keiji Kimura](http://www.imi.kyushu-u.ac.jp/eng) and Hayato Waki

Akaike's Information Criterion (AIC) is a measure of the quality of statistical model for a given set of data. We can obtain the best statistical model for the set of data by minimizing the AIC. Since this minimization is known as NP-hard, it is difficult to find the best statistical model in practice. Instead, stepwise methods, which are local search algorithms, are commonly used to find a better statistical model though it may not be the best.

We formulate this minimization with AIC as Mixed Integer Nonlinear Programming (MINLP), and propose a method to find the best statistical model. To solve this MINLP problem effectively, we implement a relaxator to find better lower bounds, heuristic algorithm to obtain better upper bounds, and branching rules for this minimization. We combine them with SCIP, which is a mathematical optimization software and a branch-and-bound framework. We show that the proposed method can provide the best statistical model for small-sized or medium-sized benchmark problems in UCI Machine Learning repository. Furthermore, we show that this method can find good quality solutions for large-sized benchmark problems.

## Call for Papers: Special Issue of Optimization Methods and Software

Papers on the topic of **MATHEMATICAL OPTIMIZATION SOFTWARE** will be considered for peer-reviewed publication in a special issue of the journal [Optimization Methods and Software](http://www.tandfonline.com/goms). The journal impact factor is 1.624, and the yearly best publication in OMS is awarded the [Charles Broyden prize](http://explore.tandfonline.com/page/est/charles-broyden-prize). The quality and topics of the submissions should correspond to the high standards of publications in OMS and its aims and scope, see http://www.tandfonline.com/action/journalInformation?show=aimsScope&journalCode=goms20.

This special issue is dedicated, but not limited to the ICMS 2016 Session on Mathematical Optimization, which was held as part of the [5th International Congress on Mathematical Software](http://icms2016.zib.de/TODO), July 11-14, 2016, at Zuse Institute Berlin.

### Guest Editors

* [Ambros Gleixner](http://www.zib.de/gleixner), Zuse Institute Berlin, Germany
* [Christian Kirches](http://www.iwr.uni-heidelberg.de/groups/optimus/people/kirches), IWR Heidelberg/TU Braunschweig, Germany
* [John Mitchell](http://www.rpi.edu/~mitchj), Rensselaer Polytechnic Institute, USA
* [Ted Ralphs](http://coral.ie.lehigh.edu/~ted), Lehigh University, USA

### Submission Guidelines

The deadline for submission to the special issue has been extended to **NOVEMBER 15, 2016**.

The authors are encouraged to keep the papers within 25 journal pages. Submissions should follow the journal's [style and guidelines](http://www.tandfonline.com/action/authorSubmission?journalCode=goms20&page=instructions).  Manuscript submission must be made online via the journal's [ScholarOne Manuscripts site](http://mc.manuscriptcentral.com/goms).

> **To specify the special issue, please choose the abbreviation "MOS" under step 5 of the submission process.**
