# bhai ki bhasha

## Notes from Research
- written in TypeScript
- will need to implement the following components:
  - lexing
    - converting text to actions - aka tokens
  - AST (abstract syntax tree)
    - represents our tokenized code 
  - parsing
    - recognize what the tokens are trying to do
  - generation
    - transforms `bhai`'s AST to `javascript`'s AST
    - module to use `escodegen`
- in the end the langauge will compile down to Javascript - and execute on the Node runtime.
- this means we must npm run the packages 
- [link to resource](https://balit.boxxen.org/overview/lexing)

### Lexing ... aka Tokenizing
- the lexer must go through token by token and interpret what is trying to be declared
- it will do this per token with no care for what it is (blindly performing our function on it)
