---
# THEME: ./DARK.JSON
author: cody_carvel@brown.edu
date: YYYY-MM-DD
paging: Slide %d / %d
---
# SHELLSAGE 

Works by understanding your terminal context

[on GitHub](https://github.com/AnswerDotAI/shell_sage)

---
# WHAT IT CLAIMS IT DOES
leverages powerful language models (Claude or GPT)
*to provide intelligent assistance for:*

- Shell commands and scripting
- System administration tasks   
- Git operations   
- File management   
- Process handling   
- Real-time problem solving   

---
# HOW IT WORKS
When you ask Shell Sage a question it can see:
- Your recent commands
- Error messages and outputs
- The current terminal content

This data along with an AI product informs Shell Sage how to help you solve problems in your shell. 

---
# WHAT SETS SHELLSAGE APART IS ITS ABILITY TO:   
   
~~Read your terminal context through tmux integration~~

~~Target specific tmux panes for focused assistance~~   

->*I will not be covering not covering tmux*->

	 *tmux is great; configuring and demoing would require more time than we have*

	 *if you use tmux, the repo README and links at the end cover this in detail*
 

Provide responses based on your current terminal state   

Accept piped input for direct analysis   

---
# INSTALL SHELLSAGE DIRECTLY FROM PYPI USING PIP:

```pip install shell_sage```

# PREREQUISITES - AN API KEY FROM ANTHROPIC OR OPENAI

Add a line in your .zshrc or .bashrc

For Claude (default) ```export ANTHROPIC_API_KEY=sk...```

For OpenAI (optional) ```export OPENAI_API_KEY=sk...```

---
# REFERENCES - LINKS

+ [Shell Sage GitHub Repo](https://github.com/AnswerDotAI/shell_sage)    
+ [ShellSage - Your AI Bash Buddy](https://www.answer.ai/posts/2024-12-05-introducing-shell-sage.html)
+ [ShellSage Loves iTerm](http://answer.ai/posts/2024-12-10-shellsage-loves-iterm.html)
+ [Why ShellSage Commands Attention](https://christhomas.co.uk/blog/2024/12/16/why-shellsage-commands-attention-in-the-ai-powered-terminal-space/)

---
# GO TO TOWN...EXAMPLES:
```ssage hi ShellSage```

---
# EXAMPLES...CSV TO JSON CONVERSION
```ssage "how can I convert a csv into a json while maintaining its original character encoding and other string formats?"```

---
# EXAMPLES...DOCKER
```cat Dockerfile | ssage "can you help me add a companion docker-compose.yml file for the Dockerfile in this directory?"```

---
# EXAMPLES...PDF > IMAGES
```ssage "how can I extract each page of a pdf as a .tiff image in its original ppi and color mode to a specific path?"```

---
# EXAMPLES...VIDEO - ADD SUBTITLES
```ssage "how can I add a .srt file into an mp4 video container?"```

---
# EXAMPLES...VIDEO - SPLIT
```ssage "how can I split an mp4 into its audio and video as separate files using ffmpeg?"```

---
# EXAMPLES...TXT CLEAN
```cat bbc_blue_planet_06_coral_seas_2001.txt | ssage "how can I remove all lines that are just a digit or digits and all lines that start and end with a digit from a .txt file and also trim whitespace and join lines with breaks into a single block of text"```

---
# EXAMPLES...TXT ADD
```ssage "how do I add the filename followed by a line break to the beginning of every txt file in this directory?"```

---
# OTHER THINGS YOU CAN DO (THAT I HAVEN'T!)

*Advanced Use Cases*

## GIT WORKFLOW ENHANCEMENT

# REVIEW CHANGES BEFORE COMMIT
```git diff | ssage summarize these changes```

# GET COMMIT MESSAGE SUGGESTIONS
```git diff --staged | ssage suggest a commit message```

# ANALYZE PR FEEDBACK
```gh pr view 123 | ssage summarize this PR feedback```

---
# MORE OTHER THINGS YOU CAN DO (THAT I HAVEN'T!)

*MORE Advanced Use Cases*

## LOG ANALYSIS

# QUICK ERROR INVESTIGATION
```journalctl -xe | ssage what's causing these errors?```

# APACHE/NGINX LOG ANALYSIS
```tail -n 100 /var/log/nginx/access.log | ssage analyze this traffic pattern```

# SYSTEM PERFORMANCE INVESTIGATION
```top -b -n 1 | ssage explain system resource usage```

---
# MORE MORE OTHER THINGS YOU CAN DO (THAT I HAVEN'T!)

*MORE MORE Advanced Use Cases*

## DOCKER MANAGEMENT

# CONTAINER TROUBLESHOOTING
```docker logs my-container | ssage "what is wrong with this container?"```

# IMAGE OPTIMIZATION
```docker history my-image | ssage suggest optimization improvements```

# COMPOSE FILE ANALYSIS
```cat docker-compose.yml | ssage review this compose configuration```

---
# YET EVEN MORE OTHER THINGS YOU CAN DO (THAT I HAVEN'T!)

*YET EVEN MORE Advanced Use Cases*

## DATABASE OPERATIONS

# QUERY OPTIMIZATION
```psql -c "EXPLAIN ANALYZE SELECT..." | ssage optimize this query```

# SCHEMA REVIEW
```pg_dump --schema-only mydb | ssage review this database schema```

# INDEX SUGGESTIONS
```psql -c "\di+" | ssage suggest missing indexes```

---
# THANKS!
