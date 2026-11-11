⚡ Black Circuit // Central de Operações & Telemetria

Black Circuit é um projeto de infraestrutura portátil (Case Mod Datacenter) desenvolvido para a ExpoTech. O projeto integra hardware em um gabinete customizado (maleta de alumínio), um servidor virtualizado em Windows Server 2022 rodando IIS 10.0, segurança perimetral via Windows Defender Firewall e um túnel HTTPS público gerenciado via ngrok.

📸 Visão Geral da Interface

A aplicação web exposta pelo servidor consiste em uma dashboard estilo SOC / Cyberpunk que simula o monitoramento da telemetria do hardware, o status de dispositivos Smart Home, logs de segurança e simulação de resposta a incidentes (Modo Lockdown).

🛠️ Stack Tecnológica

Hardware & Arquitetura: Intel Core i5-3470 @ 3.20GHz, 8 GB RAM DDR3, SSD 240GB, Maleta de Alumínio Customizada (Case Mod).

Virtualização & SO Servidor: Oracle VirtualBox, Windows Server 2022 (Desktop Experience).

Servidor Web: IIS (Internet Information Services) v10.0.

Redes & Tunelamento: TCP/IP, HTTP (Porta 80), ngrok (Reverse Proxy / HTTPS Tunneling).

Segurança Cibernética: Windows Defender Firewall (Regras de Entrada / Inbound Rules).

Frontend Web: HTML5, CSS3 (Variáveis de Tema & Responsive Layout), JavaScript Vanilla (Telemetria Simulada e Terminal de Eventos).

🔒 Destaques de Segurança Cibernética

Hardening & Princípio do Menor Privilégio: Apenas a Porta 80 (HTTP) foi liberada no Windows Defender Firewall com Segurança Avançada para receber o tráfego da aplicação web, mantendo bloqueadas portas administrativas não utilizadas.

Procedimento de Resposta a Incidentes (Lockdown): A interface possui uma rotina em JavaScript que simula o isolamento perimetral e a elevação de alerta do sistema com alteração visual instantânea e registro de auditoria no log de segurança.
