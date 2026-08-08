    1  sudo apt update && sudo apt upgrade -y
    2  sudo apt install -y build-essential git curl wget python3 python3-pip python3-venv pipx
    3  sudo apt install -y iverilog gtkwave verilator
    4  sudo apt install -y yosys nextpnr-ice40 fpga-icestorm
    5  sudo apt install -y docker.io
    6  sudo systemctl enable docker
    7  sudo systemctl start docker
    8  sudo usermod -aG docker $USER
    9  cd ~
   10  git clone https://github.com/The-OpenROAD-Project/OpenLane.git
   11  cd OpenLane
   12  make
   13  sudo apt install -y magic klayout
   14  cd..
   15  cd ..
   16  sudo apt install -y magic klayout
   17  sudo apt install -y ngspice xschem
   18  pipx install symbiyosys
   19  pipx install yowasp-yosys
   20  pipx install yowasp-yosys-smtbmc
   21  pipx install yowasp-yices
   22  sudo apt install yosys
   23  cd ~
   24  git clone https://github.com/YosysHQ/sby.git
   25  cd sby
   26  sudo make install
   27  cd ..
   28  mkdir project
   29  cd project
   30  touch adder.v
   31  vim adder.v
   32  cd ..
   33  sudo apt install vim
   34  cd project
   35  vim adder.v
   36  sudo apt update
   37  sudo apt install iverilog
   38  vim inverter.v
   39  vim inverter_tb.v
   40  iverilog -o inverter.out inverter.v inverter_tb.v
   41  vvp inverter.out
   42  :q!
   43  [200~vim inverter_tb.v~
   44  vim inverter_tb.v
   45  iverilog -o inverter.out inverter.v inverter_tb.v
   46  vim inverter_tb.v
   47  iverilog -o inverter.out inverter.v inverter_tb.v
   48  vvp inverter.out
   49  gtkwave inverter.vcd
   50  mkdir ksa_project
   51  cd ksa_project
   52  vim ksa.v
   53  vim tb_ksa.v
   54  iverilog -o ksa_out ksa.v tb_ksa.v
   55  vvp ksa_out
   56  gtkwave wave.vcd
   57  pwd
   58  ls
   59  ls-l
   60  ls -l
   61  cd VLSI_project
   62  pwd
   63  ls
   64  ls -a
   65  ls -lh
   66  ls *.v
   67  ls *.sv
   68  code .
   69  sudo apt update
   70  sudo apt install snapd
   71  sudo snap install code --classic
   72  code --version
   73  code .
   74  git clone https://github.com/Nikhilreddy0724/VLSI-Portfolio.git
   75  cd VLSI-Portfolio
   76  pwd
   77  ls
   78  git status
   79  git log --oneline
   80  cd 06_linux
   81  pwd
   82  ls
   83  mkdir Ubuntu_Practice
   84  ls
   85  cd Ubuntu_Practice
   86  pwd
   87  mkdir RTL
   88  mkdir TB
   89  mkdir Scripts
   90  mkdir Reports
   91  mkdir Logs
   92  mkdir Waves
   93  ls
   94  git status
   95  cd 06_linux
   96  mkdir Ubuntu_Practice
   97  RTL
   98  TB
   99  cd ubuntu_practice
  100  mkdir RTL
  101  mkdir TB
  102  mkdir Scripts
  103  mkdir Logs
  104  mkdir Waves
  105  ls
  106  pwd
  107  ls
  108  touch
  109  touch adder.v
  110  touch add.v or.v mux.v
  111  touch RTL/adder.v
  112  ls
  113  code mux.v
  114  git status
  115  git add .
  116  git commit -m"linux understanding"
  117  git push
  118  git config --global user.name"Nikhil Reddy"
  119  git config --global user.name "Nikhil Reddy"
  120  git config --global user.email "nikhilreddy0724@gmail.com"
  121  ping github.com
  122  git status
  123  git add .
  124  git commit -m "linux understanding"
  125  git push
  126  git remote -v
  127  git push
  128  sudo apt update
  129  sudo apt install build-essential dkms linux-headers-$(uname -r)
  130  sudo reboot
  131  cd ~/VLSSI_Portfolio
  132  cd ~/VLSI-Portfolio
  133  history
  134  history > 06_linux/Ubuntu_Practice/Ubuntu_Terminal_History.md
