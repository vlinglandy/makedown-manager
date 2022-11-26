An operating system is the software which acts as an interface between a user of a computer and the computer hardware.操作系统是计算机用户和硬件的软件接口。

The purpose of an operating system is to provide an environment in which a user execute program. 操作系统的目的是提供用户一个可以执行程序的环境。The primary goal of an operating system is thus to make the computer system convenient to use. 操作系统的主要目标因此是使计算机系统便于使用。

A secondary goal is to use the computer hardware in an efficient way. 其次是高效地使用计算机硬件。
We can view an operating system as a resource allocator. 我们可以把操作系统看做是一个资源分配器。

A computer system has many resources which may be required to solve
a problem: CPU time, memory space, file storage, input/output(I/O) devices, and so on.一个计算机系统拥有许多资源，因此需要去解决一些问题，如cpu时间，内存空间，文件存储，输入输出设备等。

The operating system acts as the manager of these resources
and allocates them to specific programs and users as necessary for their tasks. 操作系统就像是资源管理员，把资源分配给特定的程序和用户当它们工作需要时。

Since there may be many, possibly conflicting, requests for resources, the o/s must decide which requests are allocated resources to operate the computer system fairly and efficiently. 因此有可能会有很多有可能产生冲突的资源请求，操作系统必须决定分配资源给哪个请求能使计算机系统合理和有效的运行。
Early computers were(physically) very large machines run from a console.早期的计算机是从控制台运行的体积非常大的机器。

The programmer would write a program and then operate the program directly from the operator’s console. 程序员要写一条程序然
后直接从操作者的控制台操作程序。

Software such as assemblers, loaders, and compilersimproved on the convenience of programming the system, but also required substantial
set-up time. 象汇编程序、装入程序及编译程序这样的软件使系统软件编程更方便，但同时也需要大量的启动时间。To reduce the setup time, operators were hired and similarjobs were batched together.[1]为了能减少这些准备时间，操作者就被雇佣，相似的作业成批排在一起。
Batch systems allowed automatic job sequencing by a resident monitor and improve the overall utilization of the computer greatly.  批处理系统通过一个常驻内存的监控程序允许自动的作业定序。

The computer no longer had to wait for human operation.
这样计算机就不必再等待用户操作。

CPU utilization was still low, however, because of
the slow speed of the I/O devices relative to the CPU. Offline operation of slow devices was tried. 然而，CPU使用率仍然不高，这是因为I/O设备的处理速度较CPU慢导致的。

Buffering was another approach to improving system performance by overlapping the input, output, and computation of a single job. 缓冲机制是另一种提高系统系能的方法，它将一条作业的输入、输出和计算工作重叠交错进行

Finally, spooling allowed the CPU to overlap the input of one job with the computation and output of other jobs.
最后，伪脱机技术允许CPU将一条作业的输入和其他作业的计算输出交错进行。

Spooling also provides a pool of jobs which have been read and are waiting to be run. 伪脱机也为那些已经被读入并且还在等待运行的作业提供一个作业池

This job pool supports the concept of multiprogramming. 这个作业池支持一种叫做多程序设计的概念。
With multiprogramming, several jobs are kept in memory at one time;  the CPU is switched back and forth between them in order to increase CPU utilization and to decrease the total real time needed to execute a job. 在这种多程序设计技术中，多个作业可以同时存放在内存中；CPU在这些作业中来回切换控制，以至于增加CPU使用率和减少执行一条作业的总时间。

Multiprogramming, which was developed to improve performance, also allows time sharing. 多道程序设计被开发来提高性能，也允许分时。
Time-shared operating systems allow many users (from one to several hundred) to use a computer system interactive at the same time. 分时操作系统允许多个用户（从一个到几百个）同时交互式地使用计算机系统。

As the system switches rapidly from one user to the next, each user is given the impression that he has his own computer. 由于系统迅速地从一个用户切换到下一个用户，每一个用户被给予一种他拥有自己的计算机的印象。

Other operating systems types include real-time systems and multiprocessor
systems. 其他操作系统类型包括实时系统和多处理机系统。
A real-time system is often used as control de-vice in a dedicated application. 实时系统通常被用作专用的应用的控制设备。
Sensors bring data to the computer. 传感器把数据带给计算机。
The computer must analyze the data and possibly adjust controls to modify the sensor inputs. 计算机必须分析数据，也可能调整控制去修改传感器的输入。
Systems, which control scientific experiments, medical computer systems, industrial control systems, and some display systems are real-time systems. 控制科学的实验，医学的计算机系统，工业的控制系统和一些显示系统等系统都是实时系统。
A real-time operating system has well-defined fixed time constraints．实时操作系统有定义明确的固定的时间约束。
Processing must be done within the defined constraints, or the system will fail.
处理必须在定义的约束中完成，否则系统将失败。
A multiprocessor system has more than one CPU. 多处理机系统有不只一个CPU。The obvious advantages would appear to be greater computing power and reliability.显著的优势好像是强大的计算能力和可靠性。

There are various types of operating systems for multiprocessors and multicomputers.有各种各样的操作系统用于多处理机和多计算机。

It is more or less possible to distinguish two kinds of operating systems for
multiple CPU systems: Loosely coupled, such as network operating system and distributed o/s, and tightly coupled, such as parallel o/s. 这或多或少可能区分两种多CPU系统的操作系统：松耦合，例如网络操作系统和分布式操作系统，和紧耦合，如并行操作系统。

As we shall see, loosely and tightly-coupled s/w is rought analogous to loosely and tight-coupled h/w. 我们应该看到，松紧耦合软件大概类似于松紧耦合硬件。
The operating system must ensure correct operation of the computer system. 操作系统必须确保改正计算机系统的操作。
To prevent user programs from interfering with the proper operation of the system,the h/w was modified to create two modes: user mode and monitor mode 为了阻止用户程序干扰系统适当的操作，硬件被修改成两种模式：用户模式和监控模式。
Various instructions(such as I/O instructions and halt instructions) are
priviledged and can only be executed in monitor mode. 许多指令（例如I/O指令和中断指令）是有特权的，只能在监控模式下被执行。

The memory in which the monitor resides must also be protected from modification by the user. 监控程序所在的内存也必须保护起来以防用户修改。
A time prevents infinite loops. 定时器可以防止死循环。

Once these changes (dual mode,privileged instructions, memory protection, timer interrupt) have been made to the basic computer architecture, it is possible to write a correct operating system.
一旦这些对基本计算机体系结构的改变（双模，权限指令，内存保护，定时器中断）被做到，这可能写成一个改进的操作系统。
