
+++

title = "DS-RT 2024 Colloquium Slides"
description = "DS-RT 2024 Colloquium Slides"
outputs = ["Reveal"]
aliases = [
    "/ds-rt/"
]

+++

[//]: # (Narrative)
[//]: # (HCI is about balancing usability, trying to mitigate complexity / and functionality, where we add complexity)
[//]: # (Graphical User Interfaces are usually the way to interact with a PC, so they got studied to improve usability,)
[//]: # (however studies are beiong conducted to interact with different methods... also mention AR and cite)
[//]: # (simulations usually goes with a Gui, also alchemist has one)
[//]: # (Interesting outcome of LLMs to solve problems... fast)
[//]: # (multiple way to do so: configure simulations, interact with simulaor ans simulations.)
[//]: # (introduction to alchemist and its story.)
[//]: # (alchemist started of with a cli, and gradually adapted to a desktop gui,)
[//]: # (and now to a web based gui. exlain what changes at every step.)
[//]: # (can we go beyond this?)
[//]: # (let's make a parallelism with the advent of copilot in idea.)
[//]: # (example of generation of fibonacci or whatever)
[//]: # (to create a simulation of alchemist you need to know... lot of stuff, )
[//]: # (the dream is to  create something from zero and gradually ask the llm to something?)
[//]: # (How? react is an example, lot of prossibilities, research for the future)

# Evolving the Interaction with Simulators
## DS-RT 2024 - Urbino, Italy, 2024
### Angelo Filaseta - angelo.filaseta@unibo.it

---

# Interacting with Simulations

- Simulations are essential tools for *observing* complex systems and phenomena;
  - They allow to **validate** theories by comparing outcomes with expected or real-world behavior;

- *Observability* is a crucial aspect of simulations;
  - A **graphical representation** is highly beneficial for visualizing how a system evolves over time.

- *Interaction* is another key aspect;
  - essential functionalities may be *pausing*, *resuming*, *focusing on specific* parts of the simulation...

{{% multicol %}}
{{% col class="text-center"%}}
{{< figure src="eye.png" width="25%">}}
{{% /col %}}
{{% col class="text-center"%}}
{{< figure src="left-click.png" width="25%">}}
{{% /col %}}
{{% /multicol %}}

---

# What about general-purpose simulators?
- **Graphical User Interfaces (GUIs)** are usually the most practical solution in regard to general-purpose simulations.

{{% figure src="alchemist-video.gif" width="40%" %}}
<small>Alchemist Simulator - Desktop GUI __*__</small>

- Most research focus on **adding features** to GUIs while **preserving their usability**.
  - By enforcing *common design practices* it is possible to add features while keeping the interface intuitive and user-friendly.

<small>__*__ [https://alchemistsimulator.github.io/](https://alchemistsimulator.github.io/)</small>

---

# A matter of Balance

{{< figure src="balance.webp" width="10%">}}

The effectiveness of a *Human-Machine Interface (HMI)* heavenly depends on factors that can balance both ...

{{% multicol %}}
{{% col %}}
## Usability
{{% tick %}} Intuitive and user-friendly, easy to use;<br>
{{% cross %}} Usually lacking advanced features.
{{% /col %}}
{{% col %}}
## Functionality
{{% tick %}} Rich set of extensive features and capabilities;<br>
{{% cross %}} Can be overly complex to use and understand.
{{% /col %}}
{{% /multicol %}}

---

# A Case Study:  The Alchemist Simulator
{{% multicol %}}
{{% col class="col-2"%}}
{{< figure src="alchemist-logo.svg"  width="70%">}}
{{% /col %}}
{{% col class="col-10" %}}
- Alchemist<small>[5]</small> started as a **general-purpose** simulator with *Command Line Interface* and gradually introduced a *Desktop GUI*.<br>

- A new migration to a *Web GUI* is being conducted to enhance **accessibility** and **usability** even more.
  {{% /col %}}
  {{% /multicol %}}

{{< figure src="evolution.drawio.svg" width="75%">}}

<small style="text-align: left">
[5] Pianini, D., Montagna, S., & Viroli, M. (2013). Chemical-oriented simulation of computational systems with ALCHEMIST. Journal of Simulation, 7(3), 202–215.</br>
</small>

---

### Improving Human-Machine Interaction

- Diverse fields provide different solutions to improve *Human-Machine Interaction (HCI)*:

{{% multicol %}}
{{% col class="col-6" %}}
{{% centered %}}
<div class="fragment" data-fragment-index="0">

**Eye-Tracking Technology**<small> [1]</small>
{{< figure src="eyes.jpg" width="40%">}}
<small>[1] A. Poole and L. J. Ball, "Eye Tracking in HCI and Usability",<br> Research, IGI Global, 2006</small>
</div>
{{% /centered %}}
{{% /col %}}
{{% col class="col-6" %}}
{{% centered %}}

<div class="fragment" data-fragment-index="1">

**Hand Gesture Recognition**<small> [2]</small>
{{< figure src="italian-hand.jpg" width="40%">}}
<small> [2] D. Sarma and M. K. Bhuyan, “Methods, databases and recent advancement of vision-based hand gesture recognition for hci systems: A review”,<br> SN Computer Science, 2021</small>
</div>

{{% /centered %}}
{{% /col %}}
{{% col class="col-6" %}}
{{% centered %}}

<div class="fragment" data-fragment-index="2">

**Augmented Reality (AR)**<small> [3]</small>
{{< figure src="ar.jpeg" width="40%">}}
<small> [3] L. Jud, J. Fotouhi, O. Andronic, A. Aichmair, G. Osgood,
N. Navab, and M. Farshad, “Applicability of augmented reality in
orthopedic surgery – a systematic review,”<br> BMC Musculoskeletal
Disorders, 2020 </small>
</div>
{{% /centered %}}
{{% /col %}}
{{% col class="col-6" %}}
{{% centered %}}

<div class="fragment" data-fragment-index="3">

**Large Language Models (LLMs)**<small> [4]</small>
{{< figure src="llm.jpeg" width="40%">}}
<small>[4] S. Kapania, R. Wang, T. J.-J. Li, T. Li, and H. Shen, “”i’m categorizing
llm as a productivity tool”: Examining ethics of llm use in hci research
practices,” 2024.</small>
</div>

{{% /centered %}}
{{% /col %}}
{{% /multicol %}}

----

# Improving the User eXperience

<div>

- General-purpose simulators remain **inherently complex tools** due to the nature of the domains they address.
- No matter how user-friendly the interface is, *new users still need to learn how to use the simulator effectively*.
- **Domain knowledge** remains a big barrier for new users, especially if documentation is outdated<small>(😔)</small> or absent<small>(😭)</small>.

</div>


<div class="fragment pt-5" data-fragment-index="0">

## Simplifying the Learning Experience
##### and making it less boring

- Users needs a way to learn how to set-up simulations and interact with them as quickly as possible;

- Could **Large Language Models (LLMs)** enhance this assistance?

</div>

---

## Large Language Models in other contexts
### Pair Programming
{{% multicol %}}
{{% col class="col-11"%}}
- LLMs are already successfully used as **pair programming** tools (e.g. GitHub Copilot)__*__;
    - and gosh, if they can speed up the development process!
- Common applications include *code generation*, *refactoring* and *commenting*.
{{% /col %}}
{{% col class="col-1" %}}
{{< figure src="pinguin.webp" width="100%">}}
{{% /col %}}
{{% /multicol %}}

{{< figure src="copilot-example.gif" width="40%">}}
<small>__*__ Github Copilot - Your AI pair programmer: [https://github.com/features/copilot](https://github.com/features/copilot)</small>

---

# Vision - A possible application
### LLM Companion for assisting in Simulation Development

<section class="pt-5">
  <div class="container">
    <div class="row d-flex justify-content-center">
      <div class="col">
        <div class="card" id="chat1" style="border-radius: 15px;">
          <div class="card-header d-flex justify-content-between align-items-center p-3 bg-dark text-white border-bottom-0"
            style="border-top-left-radius: 15px; border-top-right-radius: 15px;">
            <i class="fas"></i>
            <p class="mb-0 fw-bold">Alchemist LLM Companion Chat</p>
            <i class="fas"></i>
          </div>
          <div class="card-body">
            <div class="fragment d-flex flex-row justify-content-start mb-4"  data-fragment-index="0">
              <img src="user.png" alt="avatar 1" style="width: 75px; height: 100%;">
              <div class="mx-3 me-3 border bg-body" style="border-radius: 15px;">
                <p class="px-3 small mb-0">Can you please generate a simulation where two devices, inside a self-organizing network, find the best path to communicate?</p>
              </div>
            </div>
            <div class="fragment d-flex flex-row justify-content-end mb-4"  data-fragment-index="1">
              <div class="p-3 me-3 border bg-body-tertiary" style="border-radius: 15px;">
                <p class="small mb-0">Sure! Here is the configuration file for the simulation you requested:</p>
              </div>
              <img src="alchemist-logo.svg" alt="avatar 1" style="width: 75px; height: 100%;">
            </div>
            <div class="fragment d-flex flex-row justify-content-end mb-4"  data-fragment-index="2">
                <img src="file.png" style="border-radius: 15px; width: 70px;">
                <img src="alchemist-logo.svg" alt="avatar 1" style="width: 75px; height: 100%;">
            </div>
            <div class="fragment d-flex flex-row justify-content-end mb-4"  data-fragment-index="3">
              <div class="p-3 me-3 border bg-body-tertiary" style="border-radius: 15px;">
                <p class="small mb-0">
                    The simulation uses the <u style="color: #39c0ed;">Collektive Incarnation</u><small>[6]</small>, an implementation
                    designed to leverage aggregate computing for modeling network behaviors.
                    I've also included the Web GUI <u style="color: #39c0ed;">Output Monitor</u>, you can view the simulation in real-time at <u style="color: #39c0ed;">localhost:8080</u>.
                    For more details about the Collektive incarnation, you can refer to the <u style="color: #39c0ed;">related documentation</u>.
                    Would you like me to run the simulation for you?
                </p>
              </div>
              <img src="alchemist-logo.svg" alt="avatar 1" style="width: 75px; height: 100%;">
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
<small>
[6] Cortecchia, A., (2024). Multiplatform Self-Organizing Systems Through a Kotlin-MP Implementation of Aggregate Computing. International Conference on ACSOS 2024.</br>
</small>
</section>


---
# Lot of Unexplored Possibilities

{{% multicol %}}
{{% col class="col-7" %}} 
- There are *many models and techniques* available for applying LLMs to specific use cases.

- An example, the **ReAct (Reason + Act)** prompting technique <small>[7]</small> focuses on generating both *reasoning traces* and *task-specific actions*.
    - Moreover, the framework is also able to retrieve information from external environments (e.g. Wikipedia).

{{< figure src="question.png" >}}
{{% /col %}}
{{% col %}}
{{< figure src="answer.png" >}}
{{% /col %}}
{{% /multicol %}}

<small>[7] S. Yao, J. Zhao, D. Yu, N. Du, I. Shafran, K. R. Narasimhan, and
Y. Cao, “React: Synergizing reasoning and acting in language models,”
in The Eleventh International Conference on Learning Representations,
ICLR 2023, Kigali, Rwanda, May 1-5, 2023. OpenReview.net, 2023.</small>

---

# Conclusion

- The inclusion of additional supporting tools in simulators could result to be very beneficial in terms of UX;
  - As of today, *LLMs* are promising tools, already used in similar contexts.

- Will simulators embrace new technologies to improve the User eXperience?
- How to *effectively design* a LLM that can assist users in interacting with simulations?
    - And what are the most important **features to include**?


{{< figure src="thinking.webp" width="10%">}}

---

# Thank you for your attention!
<small> **Angelo Filaseta** - angelo.filaseta@unibo.it</small>

{{< figure src="questions.webp" width="15%">}}

##### Some Media Attributions are required

<small>

- [Flaticon](https://www.flaticon.com/) has been used to retrieve some icons: credits to *Design Circle*, *Dimitry Miroliubov*, *Freepik*;
- [Giphy](https://giphy.com/) has been used to retrieve some gifs and stickers, credits to *Mostly ADHD Comics*, *Bratcole*, *WimpyKid*.

</small>