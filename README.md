# Project Reflection: Version Control Simulation

### Branching and Repository Management
The initial setup of this project highlighted the nuances of Git’s "unborn" branch state. While the instructions suggested cloning an empty repository and immediately branching, I recognized that Git requires a root commit to stabilize the default branch. After initializing the local repository, I managed the workflow by creating `feature/header` and `feature/footer` to isolate specific UI components. By using `git checkout -b`, I ensured that development for the header and footer remained decoupled, preventing experimental changes from affecting the stability of the `main` branch. This strategy is essential in professional environments to allow multiple developers to work on the same codebase without stepping on each's toes.

### Resolving the Merge Conflict
To simulate a real-world collision, I intentionally modified the same lines of code within `index.html` across two different branches. When attempting to merge `feature/header` into `main` after the `footer` had already been integrated, Git flagged a merge conflict. I handled this by opening the affected file, identifying the conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`), and manually selecting the desired code structure. Once the logic was reconciled, I used `git add` and `git commit` to finalize the merge. This process reinforced the importance of frequent pulls and communication within a team to minimize the complexity of these manual resolutions.

### Pull Requests and Collaboration
The transition to GitHub for the Pull Request (PR) phase demonstrated how version control shifts from a technical tool to a communication tool. By pushing the local branches and opening a PR to `review/main`, I created a transparent audit trail of the changes. The PR process is vital for code quality; it allows for peer review, where logic can be critiqued and bugs caught before they reach production. Engaging in the peer review for a classmate’s repository further emphasized this, as providing constructive feedback ensures that the entire team maintains a consistent coding standard.

### Pull Request Proofs:
![Peer Review Evidence](/dianepr.png)

![Peer Review Evidence](/josepr.png)
