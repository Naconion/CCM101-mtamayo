Stepping into Mission 10 without any step-by-step instructions was honestly intimidating at first, especially after getting used to the structured guides from our earlier labs. 
Looking back at where I started in Mission 1, just trying to get comfortable with basic Linux terminal commands, the jump to designing, deploying, and securing a complete enterprise
infrastructure from scratch feels surreal. It really forced me to stop treating these concepts as isolated assignments and start seeing how everything fits together in the real world.

The hardest part wasn't just getting the containers to run; it was making sure the whole system could actually survive on its own. Mapping out the network topology before touching any 
code helped me visualize how the host, hypervisor, and Ubuntu Server communicate. When it came time to write the docker-compose.yml file, ensuring the database used persistent volumes made
me appreciate how fragile data can be if you don't plan ahead. Locking down the server with UFW under a default-deny policy was another big reality check, it reminded me that an exposed port
is an open invitation if you're careless with security. Finally, putting together the Bash script and setting up a cron job to automate maintenance made the infrastructure feel alive, like
a system that could actually take care of itself when I'm not watching.

If there’s one major takeaway from this entire semester, it’s the mindset shift from simply following a manual to actually writing one. Troubleshooting errors without a safety net taught
me more than any tutorial ever could. Compiling everything into my GitHub repository, from the raw configuration files to the operational manual, it gives me something tangible I can actually
stand behind during the live defense. I’m walking away from this course with a much deeper, hands-on grasp of cloud engineering, security, and automation, and I feel genuinely prepared to 
build and manage real infrastructure moving forward.
