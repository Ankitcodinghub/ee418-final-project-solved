# ee418-final-project-solved
**TO GET THIS SOLUTION VISIT:** [EE418 Final Project Solved](https://www.ankitcodinghub.com/product/ee418-final-project-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;98035&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EE418 Final Project Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
2 Background

Contemporary automobiles are equipped with Electronic Control Units (ECUs) for various func- tionalities such as vehicle maneuverability and fuel efficiency etc. In order to operate these ECUs properly, the information among ECUs is exchanged via in-vehicle network protocols, such as the Controller Area Network (CAN). However, such protocols were developed for closed networks that are isolated from the external environment. Based on the closed network assumption, in-vehicle protocols were not designed for security, and in particular do not provide encryption or message authentication.

Connected vehicles, however, have an increasingly large and diverse array of outward-facing components in order to provide safety, navigation, and entertainment, which violate the assumption of a closed operating environment. These external interfaces leave connected vehicles vulnerable to attacks in which an adversary compromises one or more outward-facing ECUs (e.g., CD players or cellular radio), gains access to the CAN bus [1], and then blocks messages sent by other ECUs (i.e., denial-of-service suspension attack), sends additional fabricated messages (i.e., fabrication attack) or sends spoofed messages that claim to be originated from legitimate ECUs such as steering or engine control (i.e., masquerade attack) [2].

In this project, we consider the masquerade attack on a CAN message that is transmitted every T sec periodically, as illustrated in Fig. 1. In practice, it is difficult to detect the masquerade attack, because the frequency of the targeted message is the same before and after the attack. Nevertheless, the state-of-the-art intrusion detection system (IDS) in [2] exploits the following facts for identifying

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
2 EE 418 Autumn 2021: Network Security and Cryptography

Fig. 1. Illustration of masquerade attack. In this example, ECU A is fully compromised by the strong attacker, and ECU B is weakly compromised by the weak attacker. Before the attack, ECU B transmits message 0x11 every T sec. At t = tattack, the weak attacker suspends ECU B’s transmission of message 0x11, and the strong attacker starts fabricating and injecting spoofed messages with ID=0x11 every T sec.

ECUs: 1) ECUs operate on their local clocks without clock synchronization, and 2) the clock speed (i.e., clock skew) of an ECU is constant, and different from other ECUs. Hence, the clock skew is considered as the signature for ECUs.

3 Clock-Based Intrusion Detection System

In Part I, you will implement a clock-based IDS to detect the masquerade attack in CAN. We first review clock-related concepts, and then introduce the state-of-the-art IDS [2] and the Network Time Protocol (NTP) based IDS [3].

3.1 Clock-Related Concepts

In this project, we follow the Network Time Protocol (NTP) definitions of clocks [4]. Let us first define Ctrue as the “true” clock that runs at a constant rate, i.e., Ctrue(t) = t. Let CA(t) denote the time kept by clock A. The clock offset of CA, denoted as OA(t), is the difference between the time reported by CA and the “true” time, i.e., OA(t) = CA(t) − Ctrue(t). The frequency of CA at time t is given by CA′ (t). The clock skew of CA, denoted as SA(t), is the difference in the frequencies (or first derivatives) of CA and Ctrue, i.e., SA(t) = CA′ (t) − Ct′rue(t).

A positive clock skew means that CA runs faster than the true clock, while a negative clock skew implies that CA runs slower than the true clock. The unit of skew is microseconds per second (μs/s) or parts per million (ppm). For example, if CA is faster by 5μs every 10ms according to Ctrue, then its skew relative to Ctrue is 500ppm.

3.2 Offset Estimation

In order to use clock skew as signature for identification, an IDS (implemented at a receiving ECU) needs to first estimate average offset and accumulated offset from the arrival timestamps of a periodic message, based on which the clock skew is derived.

The average offset is estimated in batches, where each batch consists of N (e.g., 20) messages. Let the arrival timestamps in a batch be a1, a2, …, aN. We consider two ways of average/accumulated offset estimation: 1) heuristic-based [2], and 2) NTP-based [3].

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
(Strong) ECU B (Weak)

C1 11 B0

CAN Bus 11

Withoutattack C1 11 B0 C1 11 B0 C1 11 B0

Time

Withattack C1 11 B0 C1 11 B0 C1 11 B0

𝑡”##”$%

</div>
</div>
<div class="layoutArea">
<div class="column">
ECU A

</div>
</div>
<div class="layoutArea">
<div class="column">
ECU C

</div>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
–

–

</div>
<div class="column">
EE 418 Autumn 2021 Project 3

Heuristic-Based Offset Estimation: The average offset in the k-th batch is computed as:

1 􏰀N

</div>
</div>
<div class="layoutArea">
<div class="column">
3.3

</div>
<div class="column">
average offset up to the last message of the k-th batch is given by

Oacc[k] = Oacc[k − 1] + N · Oavg[k]. (4)

An example of heuristic-based and NTP-based accumulated offsets is provided in Fig. 5 in [3].

Clock Skew Estimation

</div>
</div>
<div class="layoutArea">
<div class="column">
[ai − (a1 + (i − 1)μT [k − 1])] , (1) where μT [k − 1] is the average inter-arrival time of the previous batch. The accumulated offset

</div>
</div>
<div class="layoutArea">
<div class="column">
Oavg [k] = N − 1

Oacc[k] = Oacc[k − 1] + |Oavg[k]|, (2)

</div>
</div>
<div class="layoutArea">
<div class="column">
is

where | · | in the second term of the right-hand side means the absolute value.

</div>
</div>
<div class="layoutArea">
<div class="column">
i=2

</div>
</div>
<div class="layoutArea">
<div class="column">
NTP-Based Offset Estimation: The average offset is the k-th batch is given by Oavg[k]=T−aN −a0, (3)

</div>
</div>
<div class="layoutArea">
<div class="column">
N

where a0 is the arrival timestamp of the last message in the previous batch. The accumulated

</div>
</div>
<div class="layoutArea">
<div class="column">
The accumulated offset grows linearly as a function of time, and is modeled as Oacc = S·t+e, where S is the regression parameter (i.e., clock skew), t the elapsed time, and e the identification error. To estimate the unknown parameter S, the Recursive Least Squares (RLS) algorithm is adopted:

<ol>
<li>It first computes the identification error e[k] = Oacc[k] − S[k − 1]t[k], where S[k − 1] is the estimated clock skew in the previous batch, and t[k] is the elapsed time up to the last message of the k-th batch.</li>
<li>It then updates the gain G[k] = λ−1P[k−1]t[k] , and the covariance P[k] = λ−1(P[k − 1] − 1+λ−1 t2 [k]P [k−1]G[k]t[k]P [k − 1]), where P [k − 1] is the covariance in the (k − 1)-th batch, and λ is the forgetting
factor (e.g., 0.9995).
</li>
<li>Finally, it updates the skew estimate S[k] = S[k − 1] + G[k]e[k].</li>
</ol>
3.4 Cumulative Sum (CUSUM) Detector

In a masquerade attack, the impersonating ECU has a clock skew different from the targeted ECU’s, which would lead to significant identification errors. Hence, the identification error is considered as an indicator of whether an attack is taking place. The IDS tracks the normal clock behavior for messages with the target ID by tracking the mean and variance of the errors (denoted as e), μe and σe2. To be robust against noise, μe and σe2 are updated only if the new error sample e satisfies |(e − μe)/(σe)| &lt; γ, where γ is a given update threshold (e.g., 4).

</div>
</div>
<div class="layoutArea">
<div class="column">
For detection, the CUSUM method, which derives the cumulative sums of deviations from the norm behavior, is implemented. Letting θe = e−μe , the upper and lower control limits L+ and L−

</div>
</div>
<div class="layoutArea">
<div class="column">
σe

(for detecting a sudden positive or negative shift) are updated for each new error sample as:

</div>
</div>
<div class="layoutArea">
<div class="column">
L+ =max(0,L+ +θe −κ),L− =max(0,L− −θe −κ), (5)

where κ (e.g., 8) is a sensitivity parameter. If either control limit exceeds a detection threshold Γ (e.g., 5), a sudden shift is detected, and the IDS declares an intrusion.

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
4

4

</div>
<div class="column">
EE 418 Autumn 2021: Network Security and Cryptography

Your Assignment

– Dataset: We will use the dataset collected from a real vehicle called EcoCar [5], which contains all CAN messages transmitted within 50 min (a sample screenshot is provided in Fig. 2). For our purpose, we are interested in three messages:

• 0x184: a 10-Hz message transmitted by ECU A. • 0x3d1: a 10-Hz message transmitted by ECU B. • 0x180: a 10-Hz message transmitted by ECU C.

For simplicity, we have parsed the original dataset, and generated three files (184.txt, 3d1.txt

and 180.txt), which only contain the arrival timestamps of the three messages, respectively.

<ul>
<li>– &nbsp;Scenarios: We consider two scenarios in this project.
<ul>
<li>Scenario 1 – masquerade attack: ECU A is fully compromised and ECU B is weakly compromised. The adversary stops A’s transmission of 0x184 and uses ECU B to transmit spoofed messages 0x184 every 0.1 sec instead. In practice, ECU B is transmitting 0x3d1, but we treat it as 0x184 1.</li>
<li>Scenario 2 – intelligent masquerade attack (i.e., cloaking attack): ECU A is fully compromised and ECU C is weakly compromised. A is prevented from transmitting 0x184, and C transmits spoofed message 0x184 (in practice, it is 0x180 being transmitted, but treated as 0x184). Different from Scenario 1, the adversary is intelligent and manipulates its clock skew (as seen by the detector) by adding a small time delay ∆T into message inter- departure time. That is, the adversary uses ECU C to transmit 0x184 every (0.1 + ∆T ) sec, where ∆T = −0.000029 sec or −29μs.</li>
</ul>
</li>
<li>– &nbsp;Source Code:

For Python, there are two files: ids.py and simulation.py.

<ul>
<li>ids.py: In this file, class IDS is implemented, which contains both the state-of-art and the NTP-based IDSs.</li>
<li>simulation.py: This file contains the main function and the following functions.∗ import data(file=None): Import data from file.

∗ plot acc offsets(ids, mode): ids is a dictionary that contains IDS instances, and

mode is either ’state-of-the-art’ or ’ntp-based’.

∗ simulation masquerade attack(mode): Simulate masquerade attack and plot control

limits.

∗ simulation cloaking attack(mode): Simulate cloaking attack and plot control limits.

For MATLAB, there are the following files:

<ul>
<li>IDS.m: Class IDS.</li>
<li>simulation.m: Main file for simulation.</li>
<li>import data.m: Import data from file.</li>
<li>plot acc offsets.m: Plot accumulated offset curves as function of elapsed time.</li>
<li>simulation masquerade attack.m: Simulate masquerade attack and plot control limits.</li>
<li>simulation cloaking attack.m: Simulate cloaking attack and plot control limits.</li>
</ul>
</li>
</ul>
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
1 This is mainly because ECU A is a stock ECU, and we do not want to force it to stop transmission, in order to avoid any possible damage to the real vehicle.

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
EE 418 Autumn 2021 Project 5

Fig. 2. Screenshot of collected CAN data from EcoCar [5]. Each row corresponds to a CAN message: the first entry is the arrival timestamp, followed by CAN interface ID; the last entry is the CAN message ID (in Hex) and CAN data (in Hex) that are separated by ’#’.

4.1 Tasks and Questions

<ol>
<li>Implement the class IDS.</li>
<li>Plot accumulated offset curves as function of the elapsed time for the three messages (i.e., 0x184,0x3d1 and 0x180) using the state-of-the-art IDS with batch size N = 20.</li>
<li>Repeat Task 2 for the NTP-based IDS with N = 20.– Compare the slopes of the curves from Tasks 2 and 3, and comment on the similarity of the three messages in terms of estimated clock skew from the perspective of the IDS.</li>
<li>Repeat Tasks 2 and 3 with N = 30.

– Comparing the four figures from Tasks 2 through 3, comment on the consistency of clock skewestimation (i.e., the slope of the curve for the same message should be the same regardless

of N) for the state-of-the-art and the NTP-based IDSs.
</li>
<li>Simulate the masquerade attack in Scenario 1. In this simulation, we first feed 1000 batches ofarrival timestamps of message 0x184 to the IDS, and then feed 1000 batches of arrival timestamps of message 0x3d1 to it (batch size is 20). That is, the masquerade attack occurs at the 1001-st batch, and is detected if either upper or lower control limit exceeds the threshold Γ = 5. Plot control limits as function of number of batches for the state-of-the-art and the NTP-based IDSs.
– Which IDS can detect the masquerade attack? Why?
</li>
<li>Simulate the cloaking attack in Scenario 2. In this simulation, we first feed 1000 batches of arrivaltimestamps of message 0x184 to the IDS, and then feed 1000 batches of arrival timestamps of message 0x180 to it (batch size is 20). Plot control limits as function of number of batches for</li>
</ol>
the state-of-the-art and the NTP-based IDSs.

<ul>
<li>– &nbsp;Which IDS can detect the cloaking attack? Why?</li>
<li>– &nbsp;Comparing masquerade and cloaking attacks, comment on the limitations of a clock-skewbased IDS.

Please include all necessary figures/plots, observations, and answers in your report.</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
6 EE 418 Autumn 2021: Network Security and Cryptography

4.2 Additional Questions

Read references [2] and [3], and answer the following questions.

<ol>
<li>Briefly explain how the adversary chooses ∆T for the cloaking attack on the clock skew detector.</li>
<li>What is Maximum Slackness Index (MSI), and what does it measure? Based on Fig. 8 of [3],briefly comment on the performance of cloaking attack on an IDS in terms of MSI.</li>
<li>Based on [2], explain under what circumstances, two messages are likely to be highly correlated. Based on the analysis in Section IV-C and Fig. 10 in [3], explain under what circumstances, twomessages are likely to be highly correlated.</li>
<li>Based on [3], describe how to launch the cloaking attack on the correlation detector, and brieflyexplain why it works.
Note: Please refer to [6] for an interesting and comprehensive discussion on CAN
</li>
</ol>
bus security and cloaking attack.

References

<ol>
<li>S. Checkoway, D. McCoy, B. Kantor, D. Anderson, H. Shacham, S. Savage, K. Koscher, A. Czeskis, F. Roesner, T. Kohno et al., “Comprehensive experimental analyses of automotive attack surfaces.” in USENIX Security Symposium. San Francisco, 2011.</li>
<li>K.-T. Cho and K. G. Shin, “Fingerprinting electronic control units for vehicle intrusion detection.” in USENIX Security Symposium, 2016, pp. 911–927.</li>
<li>S. U. Sagong, X. Ying, A. Clark, L. Bushnell, and R. Poovendran, “Cloaking the clock: emulating clock skew in controller area networks,” in 2018 ACM/IEEE 9th International Conference on Cyber-Physical Systems (ICCPS). IEEE, 2018, pp. 32–42.</li>
<li>S. B. Moon, P. Skelly, and D. Towsley, “Estimation and removal of clock skew from network delay measurements,” in INFOCOM’99. Eighteenth Annual Joint Conference of the IEEE Computer and Com- munications Societies. Proceedings. IEEE, vol. 1. IEEE, 1999, pp. 227–234.</li>
<li>“UW EcoCar,” http://uwecocar.com/, accessed: 2017-09-26.</li>
<li>X. Ying, S. U. Sagong, A. Clark, L. Bushnell, and R. Poovendran, “Shape of the cloak: Formal analy-sis of clock skew-based intrusion detection system in controller area networks,” IEEE Transactions on Information Forensics and Security, vol. 14, no. 9, pp. 2300–2314, 2019.</li>
</ol>
</div>
</div>
</div>
