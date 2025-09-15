# HackX-Simulator
HackX Simulator - A simulated environment for cybersecurity tools. Select a tool from the left to begin.

https://vimeo.com/1118618837?share=copy

https://gemini.google.com/share/4ee5d998c18a

HackX Simulator
HackX Simulator is a cybersecurity training and testing environment that lets users explore simulated security tools in a safe, sandboxed way. Instead of executing real exploits, HackX provides mocked, educational simulations of popular tools such as Nmap, Wireshark, and Metasploit.
Select a tool from the left (UI) to begin exploring!
🚀 Features
🛡 Safe Cybersecurity Training – no live exploits, all outputs simulated.
🔧 Multiple Tools – Simulated versions of common tools:
Nmap → port scanning simulation
Metasploit → exploit workflow simulation
Wireshark → traffic capture/analysis simulation
🌐 Configurable Environments – Load sample network topologies & traffic logs.
🧩 Extensible – Add new simulated tools by dropping them in /src/tools/.
🖥 UI Options – Command-line interface or extendable web interface.
🗂 Repository Overview
src/simulator.py → Core simulation engine
src/tool_loader.py → Loads and runs selected tools
src/tools/ → Collection of simulated cybersecurity tools
demo_data/ → Sample datasets for simulation
tests/ → Unit tests
🛠 Installation
git clone https://github.com/<your-username>/hackx-simulator
cd hackx-simulator
pip install -r requirements.txt
▶️ Usage
CLI Mode
python src/ui.py
Select a tool from the menu (e.g., Nmap, Wireshark) to run a simulated session.
Example – Nmap Simulation
>>> Select tool: Nmap
Simulated Nmap Scan Results:
Host: 192.168.0.12
 - Port 22: Open (SSH)
 - Port 80: Open (HTTP)
 - Port 443: Closed
🧪 Adding a New Tool
Create a new file in /src/tools/ (e.g., toolname_sim.py).
Implement a run_simulation() method that returns mock output.
Register your tool in tool_loader.py.
