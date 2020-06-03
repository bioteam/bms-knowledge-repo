---
title: Knowledge Repo Tutorial
authors:
- john@bioteam.net
tags:
- knowledge
- repo
- tutorial
created_at: 2020-06-03 00:00:00
updated_at: 2020-06-03 15:14:47.375968
tldr: Instructions on Knowledge Repo usage
---

## Knowledge Repo Tutorial
https://knowledge-repo.readthedocs.io/en/latest/quickstart.html

1. First, install knowledge repo toolchain using pip:


```python
!pip install --upgrade "knowledge-repo[all]"
```
2. Verify that knowledge repo has been installed:


```python
!knowledge_repo --version
```
3. Next, fork the repository at https://github.com/bioteam/bms-knowledge-repo into your own GitHub account. Clone the repository locally, modifying the username of the GitHub account to your own, in the clone URL:


```python
!git clone https://github.com/jacquayj/bms-knowledge-repo.git
```
4. Setup environment variable to allow for less verbose commands:


```python
%env KNOWLEDGE_REPO bms-knowledge-repo
```
5. Now run the command to create the knowledge post:


```python
!knowledge_repo create ipynb my_example_post3.ipynb
```
6. Save and checkpoint this tutorial notebook `File > Save and Checkpoint`, then open and modify the newly created Jupyter knowledge post in your working directory: `my_example_post.ipynb`

7. Return to this tutorial when you're finished


```python
!knowledge_repo add my_example_post3.ipynb -p project/example2 -m "test"
```

```python
!knowledge_repo submit project/example2
```