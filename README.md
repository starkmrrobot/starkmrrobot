{
  "engine": {
    "name": "starkmrrobot",
    "version": "1.0.0"
  },
  "process": {
    "name": "stark ",
    "version": "3.4"
  },
  "language": "javascript",
  "status": "success",
  "executionTime": 212, //in milliseconds
  "issues": 10, // number of identified issues
  "output": [
    // array containing all identified issues
    {
      "type": "sast", // This is static
      "ruleId": "Server Side Injection(SSI) - eval", // this is the title of the issue
      "location": {
        "path": "app/routes/contributions.js", // path to the file where the issue was identified
        "positions": {
          "begin": {
            "line": 26 // line number where the issue was identified
          }
        }
      },
      "metadata": {
        "description": "User controlled data in eval() can result in Server Side Injection (SSI) or Remote Code Execution (RCE)."
      }
    } // [...]
  ]
}