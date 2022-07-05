# Process Mining Project (a.y. 2021/2022)

##### UNICAM

###### Professor: Re Barbara

###### Student: Serpetta Damiano

---

# Introduction

Project developed by Damiano Serpetta for the Process Mining exam in University of Camerino.

The goal of the project is about to study and analyze events log in order to discover process models and checking conformance of these models.

Process Mining is entirely done by using [ProM Tool](https://www.promtools.org/doku.php).

## Process Mining

Process Mining is a methodology used to discover, monitor, and improve processes that already exist within a business by relying on data. The goal of using process mining is to explore where existing business processes are inefficient and address those critical areas.

Process Mining is fundamental for those three applications:

- Process Discovery from events log.
- Conformance of discovered processes related to event log.
- Enhancement of existing discovered processes.

## Data

The 'Hospital Billing' event log was obtained from the financial modules of the **ERP system of a regional hospital**. The event log contains events that are related to the **billing of medical services** that have been provided by the hospital. Each trace of the event log records the activities executed to bill a package of medical services that were bundled together. The event log does not contain information about the actual medical services provided by the hospital. The 100,000 traces in the event log are a random sample of process instances that were recorded over **three years**. Several attributes such as the 'state' of the process, the 'caseType', the underlying 'diagnosis' etc. are included in the event log. Events and attribute values have been **anonymized**. The time stamps of events have been randomized for this purpose, but the time between events within a trace has not been altered.

_Source_: [4TU.ResearchData](https://data.4tu.nl/)
_Data Repository_: [Hospital Billing - Event Log](https://data.4tu.nl/articles/dataset/Hospital_Billing_-_Event_Log/12705113/1)

# Log Description

<table width="95%" border="0" cellspacing="10" cellpadding="10">
<tr>
    <td width="100%" align="left" bgcolor="#AAAAAA">
    <br>
     <font face="helvetica,arial,sans-serif" size="4">Total 
    number of process instances: <b>100000</b></font><br><font face="helvetica,arial,sans-serif" size="4">Total 
    number of events: <b>451359</b></font><br>
    <font face="helvetica,arial,sans-serif" size="4">Event 
    classes defined by <b>concept:name</b></font><br><hr noshade="noshade" width="100%" size="1"><font face="arial,helvetica,sans-serif" size="+3" color="#111111">All 
    events</font>
    <br><font face="helvetica,arial,sans-serif" size="4">Total 
    number of classes: <b>18</b></font><br>

<table bgcolor="#CCCCDD" border="0" width="95%" cellpadding="4" cellspacing="2">
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4"><b>Class</b></font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4"><b>Occurrences
    (absolute)</b></font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4"><b>Occurrences
    (relative)</b></font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">NEW</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">101289</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">22,441%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">FIN</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">74738</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">16,558%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">RELEASE</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">70926</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">15,714%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">CODE OK</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">68006</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">15,067%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">BILLED</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">67448</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">14,943%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">CHANGE
    DIAGN</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">45451</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">10,07%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">DELETE</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">8225</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">1,822%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">REOPEN</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">4669</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">1,034%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">CODE NOK</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">3620</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,802%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">STORNO</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">2973</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,659%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">REJECT</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">2016</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,447%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">SET STATUS</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">705</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,156%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">EMPTY</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">449</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,099%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">MANUAL</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">372</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,082%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">JOIN-PAT</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">358</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,079%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">CODE ERROR</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">75</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,017%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">CHANGE END</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">38</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,008%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">ZDBC_BEHAN</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">1</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,0%</font>
    </td>
</tr>
</table>
<hr noshade="noshade" width="100%" size="1">
<font face="arial,helvetica,sans-serif" size="+3" color="#111111">Start
events</font><br><font face="helvetica,arial,sans-serif" size="4">Total
number of classes: <b>1</b></font><br>

<table bgcolor="#CCCCDD" border="0" width="95%" cellpadding="4" cellspacing="2">
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4"><b>Class</b></font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4"><b>Occurrences
    (absolute)</b></font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4"><b>Occurrences
    (relative)</b></font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">NEW</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">100000</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">100,0%</font>
    </td>
</tr>
</table>
<hr noshade="noshade" width="100%" size="1">
<font face="arial,helvetica,sans-serif" size="+3" color="#111111">End
events</font><br><font face="helvetica,arial,sans-serif" size="4">Total
number of classes: <b>14</b></font><br>

<table bgcolor="#CCCCDD" border="0" width="95%" cellpadding="4" cellspacing="2">
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4"><b>Class</b></font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4"><b>Occurrences
    (absolute)</b></font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4"><b>Occurrences
    (relative)</b></font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">BILLED</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">63498</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">63,498%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">NEW</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">22407</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">22,407%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">DELETE</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">8215</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">8,215%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">FIN</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">3611</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">3,611%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">CODE OK</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">948</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,948%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">SET STATUS</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">600</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,6%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">EMPTY</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">444</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,444%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">RELEASE</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">107</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,107%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">MANUAL</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">85</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,085%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">JOIN-PAT</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">47</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,047%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">CHANGE
    DIAGN</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">19</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,019%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">CODE NOK</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">14</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,014%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">REJECT</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">4</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,004%</font>
    </td>
</tr>
<tr>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">STORNO</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">1</font>
    </td>
    <td bgcolor="#CCCCCC" valign="top" align="left">
    <font face="helvetica,arial,sans-serif" size="4">0,001%</font>
    </td>
</tr>
</table>
</td>

</tr>
</table>

# Data Visualization

ProM provides some type of data visualization: _traces, events, classes, resources, attributes, and all information about the xes file._

Data Visualization provide functionalities in order to **relate various informations together**. One example is shown in the screenshot below, where we can see _Events per case_ and _Event classes per case_

_Event Log Summary Visualization_:
![Filtering Data Notebook](Screenshots/Log%20Summary%20Visualization.png)

# Filtering Data

In ProM, **event log** can be filtered in some different way, based on various attributes.

One possible filter for the event log can be represented by time: specifying a time window for traces, all traces not contained in that space-time will be deleted.

_Example of filtering data contained between 13/12/2014 and 18/01/2016_.
![Filtering Data Notebook](Screenshots/Filtering%20Data/Traces%20Filtering%20Notebook.png)

_Example of filtering data based on traces which contain event 'DELETE'_.
![Filtering Data by DELETE Event](<Screenshots/Filtering%20Data/Traces%20Visualization%20(Filtering%20by%20DELETE%20and%20view%20all%20same%20traces).png>)

Filtering Data can be done using the **Notebook Tool** in ProM, and they can be exported so that they can be used in all Process Mining actions.

### Filtering using Simple Heuristic

A way to clean data is to use the action '**Filter Log using Simple Heuristics**'. This type of ProM action has to be configured by events. Classifiers, events and types can be choosen in order to filter data.

In this case:

- All _classifiers_ are included.
- All traces which end with events 'BILLED', 'DELETE', 'FIN' o 'NEW', in state **complete**, are included.

![Filtering Data Notebook](Screenshots/Filtering%20Data/Log%20Filtered%20Data%20with%20Simple%20Heuristic.png)

# Process Mining Algorithms

Algorithms for **Process Discovery** and **Conformance Checking** are covered in this paragraph.
For this project, I choose to discover processes with 3 algorithms: **Alpha**, **Alpha+** and **Heuristic**. In particular, for the last one algorithm (_Heuristic_), **different approaches**, for _process discovery_ and _conformance checking_, are used.

## Alpha

Alpha is an Algorithm which focuses on **Control Flow**.
Relations between activities are discovered, and a **footprint table** of _direct successions_, _causality_, _parallels_ and _choices_ is calculated.

Hovewer, even if Alpha Algorithm is magnific from a sperimental and mathematic point of view, it's not suitable for real events log.

_Discovered Petri Net using Alpha_:
![Filtering Data Notebook](Screenshots/Alpha%20Miner/Alpha%20Petri%20Net.png)

In this case, we can see that it's not even close to our expectations, because of the quantity of **unconnected activities**.

## Alpha+

Alpha+ is an improved Alpha Algorithm which can discover loops of lenght of 1 and 2.

_Discovered Petri Net using Alpha+_:
![Filtering Data Notebook](Screenshots/Alpha%20Miner/Alpha%2B%20Petri%20Net.png)

Also in this case there are too much unconnected activites in this Petri Net.

We can assume that Alpha and Alpha+ are not suitable for this Events Log.

## Heuristic

Heuristic Miner is a practical applicable mining algorithm that can deal with noise, and can be used to express the main behavior (i.e. not all details and exceptions) registered in an event log.

**Two approaches** are covered in this project, based on two kind of actions in ProM.

### Approach 1: 'Mine for a Heuristic Net using Heuristic Miner'

_Configuration of Heuristic Miner action_:
![Filtering Data Notebook](Screenshots/Heuristic%20Config%201/configurations.png)

Various configurations have been tried in ProM, and this configuration gives rise to the following model.

_Discovered Model (Dependency Graph)_:
![Dependency Graph](Screenshots/Heuristic%20Config%201/Heuristic%20Dependency%20Graph.png)

With dependency graph we can also discover the related Petri Net, and consequently mapping it to a BPMN Model.

The discovered Petri Net **is not sound** and this was the main problem with this approach.

_Discovered Petri Net mapped to BPMN_:
![BPMN](Screenshots/Heuristic%20Config%201/Petri%20Net%20to%20BPMN.png)

#### Conformance Checking

Conformance Checking is done by using the action '_Replay a Log on Petri Net for Conformance Analysis_', which provides an implementation of **Alignment**.

_Conformance Checking between Model and Log_:
![Conformance Checking](Screenshots/Heuristic%20Config%201/Conformance%20Heuristic%20Dijkstra%20Visualization.png)

In ProM we can see, for each trace, the corrispondent **alignment** and **moves**.

_Alignments Sample Data_:
![Conformance Checking](Screenshots/Heuristic%20Config%201/Conformance%20Checking%20of%20DPN.png)

_Properties of Conformance Checking_:
![Conformance Checking Values](Screenshots/Heuristic%20Config%201/conformance%20checking%20values_cutted.png)

Here we can see that **Trace Fitness** is around **0.72**.

### Approach 2: 'Interactive Data-aware Heuristic Miner (iDHM)'

Second approach for Heuristic Mining is achieved by using the action '_Interactive Data-aware Heuristic Miner (iDHM)_'.

Unlike the first approach, this method is more configurable and provide to create a Petri Net which is **Sound**.

The **Approach 2** is also divided in **2 tries**.

#### First Try

First Try consists in discovering and create a simpler Model, with minor activities.

_First Model Discovered_:
![Heuristic 2 First Try](Screenshots/Heuristic%20iDHM/First%20Model%20Discovered.png)
In the right part of the screenshot, there is the **configuration** for obtaining this model, with the relative _thresholds_.

##### Conformance Checking

_ILP Alignment_:
![Heuristic 2 ILP Alignment](Screenshots/Heuristic%20iDHM/First%20Model%20Fitness%20Alignments.png)

_ILP Alignment Sample Data_:
![Heuristic 2 ILP Alignments Sample](Screenshots/Heuristic%20iDHM/First%20Model%20ILP%20Alignments%20Visualization.png)

#### Second Try

Second try is way more complicated than the first and it contains more activities.

In this case some parameters have been modified. In particular, the **Dependency Threshold** was lower, in order to get more activities in the model.

_Discovered Model with Optimal Alignments_:
![Heuristic 2 Second Try](Screenshots/Heuristic%20iDHM/Second%20Model%20Discovered%20and%20Optimal%20Alignment.png)

The relative Dependency Graph for this discovered model is obtained.

_Dependency Graph_:
![Heuristic 2 Second Try DG](Screenshots/Heuristic%20iDHM/Second%20Model%20Dependency%20Graph.png)

##### Conformance Checking

_Alignment using Splitting Replayer_:
![Alignment using Splitting Replayer](Screenshots/Heuristic%20iDHM/Second%20Model%20Fitness%20Alignments.png)

_Alignment using ILP_:
![Alignment using ILP](Screenshots/Heuristic%20iDHM/Second%20Model%20Fitness%20with%20ILP-based%20replay.png)

_ILP Alignments Sample Data_:
![ILP Alignments Sample Data](Screenshots/Heuristic%20iDHM/Second%20Model%20ILP%20Alignments%20Visualization.png)

In this second approach, we seen that we obtained a great fitness (in the first case, alignment of 1), but giving a look to alignments data, we can see that there are only _Swapped Violations_, which means that the given fitness **is not correct**.

## Social Network Analysis

In order to do **Social Network Analysis**, data has been filtered for simplicity.
In fact, in a event log composed by **100.000 traces** and **451.359 events** was a little bit difficult to interpretate resources relationships.

For the purpose of Social Network Analysis, events log was filtered taking only **100 traces** randomly, from an action of ProM.

First discovered Social Network was the Handover of Work, and in the following screenshot, we can see relationships between resources, and the respective properties like betweeness, closeness, centrality.

_Handover of Work_:
![Handover of Work](Screenshots/Social%20Network/handover%20of%20work.png)

Second discovered Social Network was the Working Together Relationship.

_Working Together Relationship_:
![Handover of Work](Screenshots/Social%20Network/working-together.png)

# Conclusions

In conclusion, I improved my capacity of understanding Logs and doing Process Mining over those. This project helps me to understand how Process Mining **works** applied to real events log and I explored the **power and functionalities** of analyzing logs to **reate Models**, **checking** its **Conformance** and doing **Social Network Analysis** on it.

I learned how a real log is formed and structured, which are its attributes and resources and which are the capabilities of _filtering data_.

I seen also the various **Process Discovery Algorithms** in practice, which are the model discovered **playing** with the **configuration**, their **conversion** to other model such as Petri Nets, and the relative **conformance checking** applied with **Alignments** between the model and the Log.

About **Process Discovery Algorithms**, i found out the differences between Alpha, Alpha+ and Heuristic.

I figured the Alpha and Alpha+ **were not suitable** for the chosen log, probably caused by _noise_, _incomplete log_ and _loops_.

The differents approaches of Heuristic Miner caught me, because of the amount of **different** possible **configurations** which lead to different models, based upon chosen **thresholds**.

About **Conformance Checking**, it helps me to understands the differences between discovered models, based on quality parameters such as **fitness**, **simplicity**, **precision** and **generalization**.
