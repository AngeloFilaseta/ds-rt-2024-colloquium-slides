
+++

title = "Guide for writing markdown slides"
description = "A Hugo theme for creating Reveal.js presentations"
outputs = ["Reveal"]
aliases = [
    "/guide/"
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

# Simulations as Testing Tools

- Simulations are essential tools for *observing* complex systems and phenomena;
- They allow to **validate** theories by comparing simulation outcomes with expected or real-world behavior;
- For this reason, *observability* is a critical aspect of simulations;

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

# Improving Interaction

Diverse fields might provide different solutions to enhance the *User Experience (UX)*
{{% multicol %}}
{{% col class="col-6" %}}
{{% centered %}}
**Eye-Tracking Technology**
{{< figure src="eyes.jpg" width="50%">}}
{{% /centered %}}
{{% /col %}}
{{% col class="col-6" %}}
{{% centered %}}
**Hand Gesture Recognition**
{{< figure src="italian-hand.jpg" width="50%">}}
{{% /centered %}}
{{% /col %}}
{{% col class="col-6" %}}
{{% centered %}}
**Augmented Reality (AR)**
{{< figure src="ar.jpeg" width="50%">}}
{{% /centered %}}
{{% /col %}}
{{% col class="col-6" %}}
{{% centered %}}
**Large Language Models (LLMs)**
{{< figure src="llm.jpeg" width="50%">}}
{{% /centered %}}
{{% /col %}}
{{% /multicol %}}

---
# What about more general-purpose simulators?
- **Graphical User Interfaces (GUIs)** are usually the most practical solution in regard to general-purpose simulations.
- Most visualization research focus on adding features to GUIs while preserving usability.
- By enforcing common design practices it is possible to add features while keeping the interface intuitive and user-friendly.

---

# The Alchemist Simulator Case
{{% multicol %}}
{{% col class="col-2"%}}
{{< figure src="alchemist-logo.svg"  width="70%">}}
{{% /col %}}
{{% col class="col-10" %}} 
- Alchemist started as a **general-purpose** simulator with *Command Line Interface* and gradually introduced a *Desktop GUI*.<br>

- A new migration to a *Web GUI* is being conducted to enhance **accessibility** and **usability** even more.
{{% /col %}}
{{% /multicol %}}

{{< figure src="evolution.drawio.svg" >}}

---

# Can we even go beyond this?

### Problems

- General-purpose simulators remain inherently complex tools due to the nature of the domains they address.
- No matter how user-friendly the interface is, new users still need to learn how to use the simulator effectively.
- *Domain knowledge* remains a big barrier for new users.

### Possible Solutions

- Assist the user as much as possible, both in the process of configuring simulations and in interacting with the simulator.
- Can Large Language Models (LLMs) help?

---

# An Example of LLM usage in Development
{{% multicol %}}
{{% col class="col-11"%}}
- LLMs are already used as **pair programming** tools (e.g. GitHub Copilot).
    - and successfully speed up the development process.
- Common applications include *code generation*, *completion*, *refactoring* and *commenting*.
{{% /col %}}
{{% col class="col-1" %}}
{{< figure src="pinguin.webp" width="100%">}}
{{% /col %}}
{{% /multicol %}}

<video width="50%" src="copilot-example.mp4" autoplay></video>

---

# Possible Vision in the Simulation Domain

<section>
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
            <div class="d-flex flex-row justify-content-start mb-4">
              <img src="user.png" alt="avatar 1" style="width: 75px; height: 100%;">
              <div class="mx-3 me-3 border bg-body" style="border-radius: 15px;">
                <p class="px-3 small mb-0">Can you please generate a simulation where two devices, inside a self-organizing network, find the best path to communicate?</p>
              </div>
            </div>
            <div class="d-flex flex-row justify-content-end mb-4">
              <div class="p-3 me-3 border bg-body-tertiary" style="border-radius: 15px;">
                <p class="small mb-0">Sure! Here is the configuration file for the simulation you requested:</p>
              </div>
              <img src="alchemist-logo.svg" alt="avatar 1" style="width: 75px; height: 100%;">
            </div>
            <div class="d-flex flex-row justify-content-end mb-4">
                <img src="file.png" style="border-radius: 15px; width: 70px;">
                <img src="alchemist-logo.svg" alt="avatar 1" style="width: 75px; height: 100%;">
            </div>
            <div class="d-flex flex-row justify-content-end mb-4">
              <div class="p-3 me-3 border bg-body-tertiary" style="border-radius: 15px;">
                <p class="small mb-0">
                    The simulation uses the <u style="color: #39c0ed;">Collektive Incarnation</u>,
                    designed to leverage aggregate computing for modeling network behaviors.
                    I've also included the Web GUI <u style="color: #39c0ed;">Output Monitor</u>, you can view the simulation in real-time at <u style="color: #39c0ed;">localhost:8080</u>.
                    For more details about the Collektive incarnation, you can refer to the <u style="color: #39c0ed;">related documentation</u>.<br>
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
</section>

---
# Lot of Unexplored Possibilities

{{% multicol %}}
{{% col class="col-7" %}} 
- There are many models and techniques available for applying LLMs to specific use cases.

- An example, the **ReAct (Reason + Act)** prompting technique focuses on generating both *reasoning traces* and *task-specific actions*.
    - Moreover, the framework is also able to retrieve information from external environments (e.g. Wikipedia).

{{< figure src="question.png" >}}
{{% /col %}}
{{% col %}}
{{< figure src="answer.png" >}}
{{% /col %}}
{{% /multicol %}}

---

# Conclusion

- The inclusion of additional supporting tools in simulators could result to be very beneficial in terms of UX;
  - As of today, *LLMs* are promising tools, already used in similar contexts.

- Will simulators embrace new technologies to improve the User eXperience?
- How to *effectively design* an LLM that can assist users in interacting with simulations?
    - And what are the most important **features to include**?


{{< figure src="thinking.webp" width="10%">}}

---

# Thank you for your attention!

{{< figure src="questions.webp" width="15%">}}

##### Some Media Attributions are required

<small>

- [Flaticon](https://www.flaticon.com/) has been used to retrieve some icons: credits to *Design Circle*, *Dimitry Miroliubov*, *Freepik*;
- [Giphy](https://giphy.com/) has been used to retrieve some gifs and stickers, credits to *Mostly ADHD Comics*, *Bratcole*, *WimpyKid*.

</small>