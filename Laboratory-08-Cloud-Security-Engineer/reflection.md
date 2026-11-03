# Reflection

A host-based firewall provides an additional layer of protection to a server even when the network's main security defenses have been bypassed. This is because it monitors and controls connections directly on the server. Even if an attacker manages to get past the router or network firewall, UFW can still block connections that are not included in its allowed rules.

Managing open network ports is important because each open port creates a possible way for attackers to access the server. If a service has security weaknesses, attackers may use them to gain unauthorized access. Closing unnecessary ports helps reduce the attack surface and makes the server more secure.

Exposing a database port such as 3306 to the public internet is risky because anyone can attempt to connect to it directly. Databases usually contain important and confidential information, making them attractive targets for attackers. Keeping database ports private helps prevent unauthorized access, password attacks, and possible exploitation of vulnerabilities.

After completing this mission, I gained a better understanding of how important server security is, especially when deploying a new server. I realized that even a newly created server can be exposed to attacks as soon as it becomes accessible online. I also learned that small mistakes, such as enabling the firewall before allowing SSH, can cause access problems, while incorrect firewall settings can leave the server vulnerable.

My GitHub portfolio now contains eight completed missions, with each activity helping me develop new cloud engineering skills. Starting from basic Linux commands in Mission 1 and progressing through infrastructure as code, monitoring, and security configuration, I can see how each mission contributes to my understanding of cloud infrastructure. Overall, my portfolio shows my progress from learning basic concepts to applying practical cloud engineering and security techniques.
