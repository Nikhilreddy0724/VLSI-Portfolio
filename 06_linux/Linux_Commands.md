# Linux Interview Commands

## 1. pwd
### Meaning
Print Working Directory.

### Syntax
pwd

### Example
pwd

### Use in VLSI
Used to verify the current project directory before compilation or simulation.

---

## 2. ls
### Meaning
List directory contents.

### Examples
ls
ls -l
ls -la
ls -lh

### VLSI Use
Used to inspect RTL, testbench, log and report files.

---

## 3. cd
### Meaning
Change directory.

### Examples
cd RTL
cd ..
cd ~
cd -

---

## 4. mkdir
### Meaning
Create directory.

### Example
mkdir RTL

### VLSI Use
Used to create project directories.

---

## 5. touch
### Meaning
Create an empty file or update timestamps.

### Example
touch alu.v

### VLSI Use
Create RTL, testbench and script files.

---

## 6. cp
### Meaning
Copy files/directories.

### Example
cp alu.v Backup/

---

## 7. mv
### Meaning
Move or rename files.

### Example
mv alu.v RTL/

---

## 8. rm
### Meaning
Remove files.

### Example
rm test.txt

### Warning
Use carefully because deleted files may not be recoverable.

---

## 9. cat
### Meaning
Display file contents.

### Example
cat simulation.log

---

## 10. less
### Meaning
Read large files page by page.

### Example
less simulation.log

---

## 11. head
### Meaning
Display beginning of a file.

### Example
head -n 20 simulation.log

---

## 12. tail
### Meaning
Display end of a file.

### Example
tail -n 20 simulation.log

### VLSI
tail -f simulation.log

Used to monitor a growing simulation log.

---

## 13. find
### Meaning
Search files/directories.

### Example
find . -name "*.v"

---

## 14. grep
### Meaning
Search text patterns.

### Examples
grep "ERROR" simulation.log
grep -i "warning" simulation.log
grep -r "ERROR" Logs/

### VLSI
Used extensively for searching errors/warnings in EDA logs.

---

## 15. wc
### Meaning
Count lines, words and characters.

### Examples
wc -l file.txt
wc -w file.txt
wc -m file.txt

---

## 16. chmod
### Meaning
Change file permissions.

### Example
chmod +x run.sh
chmod 755 run.sh

---

## 17. ps
### Meaning
Display processes.

### Example
ps aux

---

## 18. top
### Meaning
Interactive process/resource monitor.

### Example
top

---

## 19. kill
### Meaning
Terminate a process.

### Example
kill PID

---

## 20. df
### Meaning
Display filesystem disk usage.

### Example
df -h

---

## 21. du
### Meaning
Display directory/file size.

### Example
du -sh project/

---

## 22. free
### Meaning
Display memory usage.

### Example
free -h

---

## 23. history
### Meaning
Display previously executed commands.

### Example
history
history | grep git

---

## 24. echo
### Meaning
Print text or variables.

### Examples
echo "Hello"
echo $PATH

---

## 25. man
### Meaning
Display command manual.

### Example
man grep

---

## 26. Pipe |
### Meaning
Pass output of one command to another.

### Example
ps aux | grep vvp

---

## 27. >
### Meaning
Redirect output and overwrite file.

### Example
ls > files.txt

---

## 28. >>
### Meaning
Append output to a file.

### Example
ls >> files.txt

---

## 29. ssh
### Meaning
Secure remote shell connection.

### Example
ssh user@server

### VLSI
Used to access remote Linux/EDA servers.

---

## 30. scp
### Meaning
Securely copy files between machines.

### Example
scp alu.v user@server:/home/user/RTL/

---

## 31. tar
### Meaning
Create/extract archives.

### Examples
tar -cvf project.tar project/
tar -xvf project.tar

---

## 32. export
### Meaning
Set environment variables.

### Example
export PROJECT=VLSI

---

## 33. which
### Meaning
Show executable location.

### Example
which iverilog

---

## 34. ip
### Meaning
Network configuration command.

### Examples
ip addr
ip route

---

## 35. apt
### Meaning
Ubuntu package management.

### Examples
sudo apt update
apt search iverilog
sudo apt install iverilog

---

## 36. make
### Meaning
Build/automation tool.

### Examples
make
make clean

### VLSI
Can automate RTL compilation and simulation.

---

# VLSI-Specific Commands

## iverilog

Compile Verilog:

iverilog -o sim RTL/and_gate.v TB/and_gate_tb.v

## vvp

Run compiled simulation:

vvp sim

## gtkwave

View waveform:

gtkwave and_gate.vcd

## make

Automate compilation and simulation.

## grep

Search simulation logs.

## find

Locate RTL/testbench files.

## tail

Monitor simulation logs.

## chmod

Make scripts executable.

## ps

Monitor EDA/simulation processes.

## kill

Terminate stuck processes.

## ssh

Access remote EDA servers.

## scp

Transfer RTL/scripts/results between machines.
