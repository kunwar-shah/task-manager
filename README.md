# Task Manager Application - Chapter 1: Project Setup and Version Control  
This branch covers the initial setup of our Task Manager application, including development environment setup and version control initialization.

## Key Points: 
- Project initialization with npm
- Git repository setup
- GitHub integration
- Introduction to asynchronous JavaScript in Node.js
## Branch Features:
- Basic project structure
- package.json file
- .gitignore file
- Initial commit

## Setup Instructions:  
1. Clone the repository:
 ```bash
git clone https://github.com/yourusername/task-manager.git
cd task-manager
```
2. Switch to this chapter's branch:
```bash
git checkout chapter-1-setup
```
3. Initialize the project:
```bash
npm init -y
```
4. Set up Git:
```bash
git init
```
5. Create .gitignore:
```bash
echo "node_modules/\n.env" > .gitignore
```
6. Set up GitHub repository:
```bash
git remote add origin https://github.com/yourusername/task-manager.git
git branch -M main
```
7. Ensure MongoDB is running on your local machine (using Laragon in our case)

## Asynchronous JavaScript 
Example:  
```javascript 
console.log('Start');
setTimeout(() => {
console.log('This is asynchronous');
}, 0);
console.log('End');
```
This demonstrates the asynchronous nature of Node.js. 

## Next Steps: 
The next chapter will focus on setting up the application architecture and folder structure, implementing MVC for both frontend and backend. 
