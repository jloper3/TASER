
# TASER
Welcome to your **personal AI Executive Assistant** — the system that **plans, decomposes, and procures tasks like a pro**, while keeping you in control and making the console **look awesome**. 🚀

---

## ✨ Features That Will Make You Smile

* **🧑‍💼 Executive Assistant Orchestrator**
  The big boss of the system. Refines your goals, applies constraints, and keeps everything moving smoothly.

* **📝 Planner Agent**
  Breaks down your master goals into sub-goals and tasks. Each task comes with metadata so you always know:

  * ✅ **Atomic** – ready to execute
  * ❌ **Non-Atomic** – needs some love (aka decomposition)
  * ⚠️ **Side-Effect** – modifies external systems, handle with care

* **⚙️ Procurement Agent**
  Turns tasks into **actionable “how-to” instructions**, while respecting atomicity and side-effect flags.

* **🎨 Rich Console Interface**
  Beautiful tables, colored panels, clear visual cues — tasks jump off the screen!

* **🔄 Stateful Feedback Loop**
  Revise, iterate, refine — the system remembers your feedback and improves automatically.

---

## 🛠 Installation (Get Started Fast)

```bash
git clone <repo-url>
cd interactive-planning-assistant
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
pip install -r requirements.txt
```

**Dependencies**:

* Python 3.10+
* [LangGraph](https://pypi.org/project/langgraph/)
* [Rich](https://pypi.org/project/rich/)

---

## 🗂 Project Structure

```
interactive-planning-assistant/
│
├─ agents/
│  ├─ executive_assistant_interactive_rich_full.py
│  ├─ planner.py
│  └─ procurement_agent.py
│
├─ main.py
├─ requirements.txt
└─ README.md
```

---

## 🚀 How to Use

```bash
python main.py
```

1. Enter your **master goal** (e.g., “Launch a Python course with \$500 in 3 weeks”).
2. Review the **Planner output** in a gorgeous Rich table.

   * Accept it ✅ or provide revision feedback ✏️
3. Review the **Procurement output** with detailed instructions.
4. Iterate until all tasks are approved.
5. Celebrate 🎉 — your final outputs are ready to rock.

---

## 🧩 Task Metadata (Because Knowledge is Power)

| Field         | Description                                      |
| ------------- | ------------------------------------------------ |
| `atomic`      | ✅ Ready-to-go task, ❌ Compound task              |
| `side_effect` | ⚠️ Modifies external systems, ✅ Safe             |
| `subtasks`    | Optional breakdown of compound tasks             |
| `how`         | Step-by-step instructions from Procurement Agent |

Example:

```yaml
- name: "Send welcome emails"
  atomic: true
  side_effect: true
  how: "Use Mailchimp API to send emails 🎯"
```

---

## 🎨 Interactive Features

* **Rich panels & tables** for Planner and Procurement outputs
* **Color-coded** tasks for instant scanning
* **Automatic feedback loops** that learn from your revisions
* **Side-effect alerts** so you never break anything by accident 😅


---

