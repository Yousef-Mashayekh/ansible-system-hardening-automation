# Linux-System-Hardening-Automation

that applies three core security controls (firewalld, SELinux, and Fail2ban) across client systems.  The playbook is parametric, meaning its behavior is driven by variables rather than hardcoded values, allowing it to be reused indefinitely by simply adjusting inputs instead of rewriting logic. To ensure safe rollout, I created a dedicated test group and validated the role’s behavior there before applying it to production systems. I also added granular task tagging, giving operators the ability to run only specific components without executing the entire hardening workflow. This adds modularity, control, and operational flexibility.
Idempotency, was confirmed so that repeated runs don't introduce unintended changes, Fail2ban’s integration with firewalld was also validated, ensuring bans are correctly enforced at the firewall level.

