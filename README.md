
## 1. Configuración de red
<img width="1912" height="976" alt="red-interna" src="https://github.com/user-attachments/assets/e8cf8ec4-3376-423e-b2dc-2436e532dadf" />
## 2. Justificación técnica
Configuré el adaptador de red de la máquina virtual en modo Red interna porque, en esta etapa del laboratorio, la VM no necesita salir a internet ni comunicarse con mi equipo real. En este modo, la VM solo puede comunicarse con otras máquinas conectadas a la misma red interna de VirtualBox, lo que la deja aislada del anfitrión, de mi red doméstica y de internet. Esto reduce la superficie de ataque y permite contener cualquier comportamiento inesperado dentro del laboratorio. No usé el modo Puente (Bridged) porque conecta la VM directamente a mi red física: recibiría una IP de mi router y se comportaría como un dispositivo más de la casa. Eso expondría mi laboratorio a los demás equipos de la red doméstica y, a la inversa, cualquier prueba o software riesgoso que ejecute en la VM podría alcanzar esos dispositivos. Instalé las Guest Additions con NAT, antes de aislar la VM, porque requieren internet.
## 3. Snapshot inicial
<img width="1917" height="588" alt="snapshot" src="https://github.com/user-attachments/assets/1023ad0c-1c24-49e2-aa81-1412e281444c" />
