> 🏗️ **Self-Hosted First:** My primary infrastructure workflows, homelab orchestrations, and internal CI/CD pipelines run on a self-hosted GitOps stack (Forgejo / GitLab), mirrored selectively to GitHub.

<h3 align="center">
  Hey there, nice to see you here! 👋
</h3>

<p align="center">
  <a href="#"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&duration=4000&pause=1000&color=CA3571&center=true&vCenter=true&width=460&lines=Red+Hat+Certified+System+Administrator;SysOps+Engineer;Network+Engineer;Big+Tech+Lover" /></a>
</p>

<div>
  <h2>⚡️ A Few Quick Facts</h2>
  <img width="400px" align="right" src="https://user-images.githubusercontent.com/85310475/209472552-ee8c70ff-050d-45cf-a3bd-e300f5b976cf.jpg" />
  <ul>
    <li>🎓 <strong>Certifications:</strong> Red Hat Certified System Administrator (RHCSA), Fortinet NSE, Scrum SFC.</li>
    <li>☁️ <strong>Enterprise Focus:</strong> Cloud & SysOps Engineering, Linux Systems (RHEL / Debian), OpenTofu / Terraform IaC, Ansible.</li>
    <li>🖥️ <strong>Homelab & Virtualization:</strong> Multi-node Proxmox VE cluster with 10G SDN, ZFS/ZRAM, PBS offsite backups, and automated DR.</li>
    <li>👨‍💻 More information and live architecture on <a href="https://speedrapide10.github.io/">my portfolio website</a>.</li>
    <li>📝 Connect with me on <a href="https://www.linkedin.com/in/oussama-karem/">LinkedIn</a>.</li>
    <li>💬 Passionate about Infrastructure as Code, Linux kernel tuning, high-availability clusters, and GitOps automation.</li>
  </ul>
</div>

<br clear="all" />

<div>
  <h2>🧑‍💻 Featured Projects & Architecture</h2>
  <table width="100%">
    <tr>
      <td width="50%" valign="top">
        <h3><a href="https://github.com/speedrapide10/Tailscale-ACL">🔐 Tailscale Zero-Trust GitOps</a></h3>
        <p>Automated network access control and continuous deployment pipeline using GitHub Actions, Tailscale ACLs, and HuJSON policies.</p>
        <ul>
          <li>Automated CI/CD validation via GitHub Actions</li>
          <li>Granular Zero-Trust RBAC grants & subnet router isolation</li>
        </ul>
        <p>
          <img src="https://img.shields.io/badge/Tailscale-Zero--Trust-blue?style=flat-square&logo=tailscale" />
          <img src="https://img.shields.io/badge/CI%2FCD-GitHub_Actions-2088FF?style=flat-square&logo=githubactions" />
          <img src="https://img.shields.io/badge/Security-RBAC-green?style=flat-square" />
        </p>
      </td>
      <td width="50%" valign="top">
        <h3><a href="https://github.com/speedrapide10/portainer-stacks-backup">🐳 Portainer & Docker DR Engine</a></h3>
        <p>Zero-touch automated backup and disaster recovery engine for multi-host Docker/Portainer environments with Mattermost observability.</p>
        <ul>
          <li>Automated Git delta synchronization to self-hosted Forgejo</li>
          <li>Real-time failure alerting via embedded Mattermost webhooks</li>
        </ul>
        <p>
          <img src="https://img.shields.io/badge/Docker-Portainer-2496ED?style=flat-square&logo=docker" />
          <img src="https://img.shields.io/badge/Bash-Automation-4EAA25?style=flat-square&logo=gnu-bash" />
          <img src="https://img.shields.io/badge/Forgejo-GitOps-FB923C?style=flat-square&logo=forgejo" />
        </p>
      </td>
    </tr>
    <tr>
      <td width="50%" valign="top">
        <h3><a href="https://github.com/speedrapide10/Proxmox-Public-Scripts">🖥️ Proxmox VE Automation Suite</a></h3>
        <p>Production-tested maintenance, kernel scheduling, and storage optimization scripts for enterprise Proxmox hypervisors.</p>
        <ul>
          <li>VirtIO SCSI storage tuning, hardware TRIM & ZRAM swappiness</li>
          <li>Automated Proxmox Backup Server (PBS) prune & GC lifecycle</li>
        </ul>
        <p>
          <img src="https://img.shields.io/badge/Proxmox-VE-E57000?style=flat-square&logo=proxmox" />
          <img src="https://img.shields.io/badge/Linux-Kernel-FCC624?style=flat-square&logo=linux" />
          <img src="https://img.shields.io/badge/Storage-VirtIO_SCSI-red?style=flat-square" />
        </p>
      </td>
      <td width="50%" valign="top">
        <h3><a href="https://github.com/speedrapide10/docker-cloudflare-ddns">☁️ Cloudflare Dynamic DNS</a></h3>
        <p>Edge DNS management and dynamic IP synchronization container for multi-WAN and home-lab gateway infrastructure.</p>
        <ul>
          <li>Zero-downtime edge IP failover with healthchecks</li>
          <li>Multi-network support for resilient WAN gateway routing</li>
        </ul>
        <p>
          <img src="https://img.shields.io/badge/Cloudflare-DNS-F38020?style=flat-square&logo=cloudflare" />
          <img src="https://img.shields.io/badge/Docker-Edge-2496ED?style=flat-square&logo=docker" />
          <img src="https://img.shields.io/badge/Network-High_Availability-blue?style=flat-square" />
        </p>
      </td>
    </tr>
    <tr>
      <td colspan="2" valign="top">
        <h3><a href="https://github.com/speedrapide10/my-code-server">💻 Cloud Development Workspace</a></h3>
        <p>Self-contained development environment in Docker with customized tooling, extensions, and persistent secure storage.</p>
        <p>
          <img src="https://img.shields.io/badge/VS_Code-Server-007ACC?style=flat-square&logo=visualstudiocode" />
          <img src="https://img.shields.io/badge/Docker-Compose-2496ED?style=flat-square&logo=docker" />
        </p>
      </td>
    </tr>
  </table>
</div>

<div>
  <h2>🏗️ Homelab Architecture Overview</h2>
  <pre>
┌────────────────────────────────────────────────────────────────────────┐
│                       CLOUDFLARE ZERO-TRUST EDGE                       │
└───────────────────────────────────┬────────────────────────────────────┘
                                    │ WireGuard / Tailscale Mesh
┌───────────────────────────────────┴────────────────────────────────────┐
│                   SPEEDXNIGHT CLUSTER INFRASTRUCTURE                   │
├────────────────────────┬────────────────────────┬──────────────────────┤
│      PROXMOX VE 1      │      PROXMOX VE 2      │     PROXMOX VE 3     │
│ [Monkey] i3-6100T/24G  │ [Beast] Core i7 / 32G  │ [Spike] Core i5/16G  │
├────────────────────────┼────────────────────────┼──────────────────────┤
│ • OMYV Storage NAS     │ • Production Docker    │ • Staging Lab & DR   │
│ • VPBS Backup Server   │ • Mattermost Webhooks  │ • PBS Remote Target  │
│ • Corosync Ring 0/1    │ • Forgejo GitOps Hub   │ • Fail2ban nftables  │
│ • Dedicated VLAN 3288  │ • Portainer Stacks     │ • Network Watchdogs  │
└────────────────────────┴────────────────────────┴──────────────────────┘
  </pre>
</div>

<h2>📊 Contribution Activity</h2>

<p align="center"> 
  <img src="https://streak-stats.demolab.com?user=speedrapide10&theme=radical&hide_border=true" alt="GitHub Streak Stats" />
</p>

<h2>🛠️ My favorite tools</h2>

### My used programming and scripting languages

<p>
  <a href="https://github.com/search?q=user%3Aspeedrapide10+Bash"><img alt="Bash" src="https://img.shields.io/badge/Bash-4EAA25?logo=gnu-bash&logoColor=white&style=for-the-badge"></a>
  <a href="https://github.com/search?q=user%3Aspeedrapide10+HTML5"><img alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white&style=for-the-badge"></a>
  <a href="https://github.com/search?q=user%3Aspeedrapide10+Markdown"><img alt="Markdown" src="https://img.shields.io/badge/Markdown-000000?logo=markdown&logoColor=white&style=for-the-badge"></a>
  <a href="https://github.com/search?q=user%3Aspeedrapide10+Python"><img alt="Python" src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white&style=for-the-badge"></a>
</p>

### My used software and tools
<p>
  <a href="#"><img alt="AWS" src="https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white" /></a>
  <a href="#"><img alt="Proxmox" src="https://img.shields.io/badge/proxmox-proxmox?style=for-the-badge&logo=proxmox&logoColor=%23E57000&labelColor=%232b2a33&color=%232b2a33" /></a>
  <a href="#"><img alt="Debian" src="https://img.shields.io/badge/Debian-D70A53?style=for-the-badge&logo=debian&logoColor=white" /></a>
  <a href="#"><img alt="RedHat" src="https://img.shields.io/badge/Red%20Hat-EE0000?style=for-the-badge&logo=redhat&logoColor=white" /></a>
  <a href="#"><img alt="Ansible" src="https://img.shields.io/badge/ansible-%231A1918.svg?style=for-the-badge&logo=ansible&logoColor=white" /></a>
  <a href="#"><img alt="Terraform" src="https://img.shields.io/badge/terraform-%235835CC.svg?style=for-the-badge&logo=terraform&logoColor=white" /></a>
  <a href="#"><img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white&style=for-the-badge" /></a>
  <a href="#"><img alt="Git" src="https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white&style=for-the-badge" /></a>
  <a href="#"><img alt="Forgejo" src="https://img.shields.io/badge/forgejo-%23FB923C.svg?style=for-the-badge&logo=forgejo&logoColor=white" /></a>
  <a href="#"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=white&style=for-the-badge" /></a>
  <a href="#"><img alt="Kali Linux" src="https://img.shields.io/badge/Kali%20Linux-557C94?logo=kali-linux&logoColor=white&style=for-the-badge" /></a>
  <a href="#"><img alt="Visual Studio Code" src="https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?logo=visual-studio-code&logoColor=white&style=for-the-badge" /></a>
  <a href="#"><img alt="ChatGPT" src="https://img.shields.io/badge/chatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white" /></a>
  <a href="#"><img alt="Cloudflare" src="https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=Cloudflare&logoColor=white" /></a>
  <a href="#"><img alt="GitHub Pages" src="https://img.shields.io/badge/github%20pages-121013?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="#"><img alt="Linode" src="https://img.shields.io/badge/linode-00A95C?style=for-the-badge&logo=linode&logoColor=white" /></a>
</p>

### My favorite sources/forums
<p>
  <a href="#"><img alt="Reddit" src="https://img.shields.io/badge/Reddit-%23FF4500.svg?style=for-the-badge&logo=Reddit&logoColor=white" /></a>
  <a href="#"><img alt="Stack Overflow" src="https://img.shields.io/badge/-Stack%20Overflow-F58025?logo=stack-overflow&logoColor=white&style=for-the-badge" /></a>
  <a href="#"><img alt="Medium" src="https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white" /></a>
  <a href="#"><img alt="StackExchange" src="https://img.shields.io/badge/StackExchange-%23ffffff.svg?style=for-the-badge&logo=StackExchange" /></a>
  <a href="#"><img alt="XDA Developers" src="https://img.shields.io/badge/XDA--Developers-%23AC6E2F.svg?style=for-the-badge&logo=XDA-Developers&logoColor=white" /></a>
  <a href="#"><img alt="Dev.to" src="https://img.shields.io/badge/dev.to-0A0A0A?style=for-the-badge&logo=dev.to&logoColor=white" /></a>
</p>

Made with ❤️ by Oussama
