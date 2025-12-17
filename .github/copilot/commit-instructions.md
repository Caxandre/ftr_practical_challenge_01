Create a commit message strictly following the Conventional Commits specifications (https://www.conventionalcommits.org/). The message must:

1. Follow the structure: <type>[(optional scope)]: <description>

2. Valid commit types:

   - fix: bug fixes
   - feat: new features
   - docs: documentation changes
   - style: formatting that does not affect code logic
   - refactor: refactoring that does not add features
   - test: addition or correction of tests
   - chore: changes in tools, configurations, etc.

3. Optional scope (in parentheses) to indicate the specific affected area
   Example: feat(authentication): add JWT authentication

4. Clear and concise description in imperative mood, starting with lowercase
   Maximum of 72 characters

5. Message body (optional) for more detailed explanations:

   - Use a blank line after the title
   - Describe the reason for the changes
   - Explain impacts or important considerations

6. Footer (optional) to reference issues or breaking changes
   Example: Closes #123, BREAKING CHANGE: API modified

Complete example:

````feat(user-management): add password reset function

Implements complete password recovery flow
- Sends email with reset link
- Validates recovery token
- Updates user password

Closes #456```
````
