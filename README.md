# computer-architecture-assignment-3-solved
**TO GET THIS SOLUTION VISIT:** [Computer Architecture Assignment 3 Solved](https://www.ankitcodinghub.com/product/computer-architecture-laboratory-assignment-3-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117892&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Computer Architecture Assignment 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
Develop a single cycle processor simulator for ToyRISC.

Input to the Program

1. full path to the configuration file. A sample file is given at src/configuration/config.xml. This describes the processor to be simulated. This is not of much use in this assignment, but will be utilized in coming assignments.

2. full path to the statistics file to be created. This file contains the statisticsof the simulation run – number of instructions executed, number of cycles taken, etc.

3. full path to the object file whose execution is to be simulated.

Output of the Program

• the program must create the statistics file at the specified location.

Broad Outline of the Steps

• The source is available at gitea. git clone https://gitea.iitdh.ac. in:443/rajshekar.k/CS311_assignment3.git

• Loading of the program: Begin with implementing the loadProgram function in the file Simulator.java. Store the global data and instructions in the approporiate locations in the mainMemory structure (see Section “Address Space Layout” in assignment 1). Set the PC register to the memory address of the first instruction (remember from assignment 2 that this is the first integer in the object file). Set x0= 0, x1= 216 − 1, and x2= 216− 1.

You can check the contents of the memory using processor.getMainMemory() .getContentsAsString(&lt;starting-address&gt;, &lt;ending-address&gt;).

• Simulation of the program:

– The function simulate() in the file src/generic/Simulator.java describes the overall loop that captures the simulation. The five stages of the processor are called in-order.

1

– As discussed in class, between every two stages, there is a latch. The contents of the different latches are obviously different. Therefore, for each latch type, a separate class has been created. For example, the

IF-OF latch is described by the file src/processor/pipeline/IF OF LatchType.java. An object of this type is created, and references to the same object are given to both the IF stage and the OF stage.

You have to decide the contents of each latch. IF OF LatchType has been done for you. Similarly, implement the remaining latches.

– Implement each of the stages. The IF stage has been implemented for you. Similarly, implement the remaining stages.

– The simulation ends when an end instruction passes through the IF stage. Call setSimulationComplete() (defined in the file src/generic/Simulator.java) at this point.

• Tabulate cycles and instruction counts for all programs that you submitted as part of assignment 1, in your report. These programs will function as benchmarks for the our processor designs.

Testing

Five example ToyRISC programs, their object codes, and the corresponding expected system state at the end of execution, are given in the supporting files archive. Also, the simulator prints a hash value – a hash of the processor state – at the end of the execution. The expected correct hash values are also given.

Run python test zip.py &lt;path to zip file&gt; to check your submission.

Follow the same naming convention: “&lt;roll-number-1&gt;&lt;roll-number-2&gt; assignment3.zip”.

Note

• All subsequent assignments in this course will involve modifying this set of source files. You will be adding many more files to this project. Please use version controlling extensively, and back up your code frequently.

• You will have two weeks to submit this assignment.

2
