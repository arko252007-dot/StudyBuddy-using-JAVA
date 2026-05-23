# StudyBuddy (Console-based Interactive Chatbot Engine)

An interactive, command-line utility designed to assist students during long study sessions. The application features contextual time-of-day parsing, a dynamic keyword evaluation engine, simulated asynchronous latency, and adaptive string-formatting algorithms.

## 🚀 Key Technical Features

* **Contextual Greeting System:** Utilizes `java.time.LocalTime` and native formatting utilities to fetch system architecture time, parsing real-time hours into customized, localized greetings (Morning, Afternoon, Evening, and Late-Night variations).
* **Robust Input Sanitization:** Processes individual user strings using character trimming, case-normalization (`toLowerCase`), dynamic boundary substring manipulation, and string capitalization metrics.
* **HashMap Keyword Routing Engine:** Employs a `HashMap<String, String>` mapping framework. Features a linear-search keyword containment protocol (`.contains()`) that maps user contexts to specific pre-allocated responses.
* **Simulated Latency Overhead:** Integrates thread state management (`Thread.sleep`) to mock real-world processing latency, creating a natural interaction interface.
* **Dynamic Content Interpolation:** Custom runtime string parsing conditionally injects variables (such as the user's name or dynamic timestamps) into static memory maps using data streams.

---

## 🛠️ Architecture & Core Components Used
* **Language:** Java (JDK 8+)
* **Data Structures:** `java.util.HashMap`, `java.util.Map`
* **Input Streams:** `java.util.Scanner`
* **Date-Time API:** `java.time.LocalTime`, `java.time.format.DateTimeFormatter`
* **Concurrency:** Thread-safe execution using exception catch-blocks (`InterruptedException`)

---

## 💻 How to Run the Pre-compiled Executable

### Prerequisites
Ensure you have the Java Runtime Environment (JRE) installed. You can check by running:
```bash
java -version

Execution Steps
    1. Clone or download only the compiled StudyBuddy.jar artifact from this repository.

    2. Open your terminal or system command prompt and navigate to the directory holding the downloaded file.

    3. Fire up the application using the standalone deployment flag:
        java -jar StudyBuddy.jar