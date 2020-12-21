# NEON-Cipher-Conky.conf-FIXED
Converted the conky.conf from http://neoncipher.net/v/conky/

Origional file setup credit goes to Neon Cipher.
I just converted it to be compatible with the newer syntax.

Just remember to change the title, your network adapter name, and how many cores for your system.
My conf is set up for an 8 core CPU

If you want a GPU Utilization bar (Nvidia only) plug this in where you'd like under the text section

${font Arial:bold:size=10}${color #3b71a1}GPU ${color #3b71a1}${hr 2}
${execbar nvidia-smi -q -d utilization | awk '/Gpu/{i++}i==1{print $3; exit}'}
