# **How to use**
the training data is one array and the prediction generates "branches" of input output links, using an array of scored outputs to derive the next most fitting phrase

right now the model has one way to prompt, which takes your prompt and predicts the next most fitting phrases for a given amount of iterations. this model does not use proper training methods or artificial neurons, and does not work on a token level but instead phrase-by-phrase.
```js
window.Jabba.predict(prompt,outputLength); //returns the jabba.js prediction of next words as a string

//output length is 5 by default, which makes a decent sized chunk of text
```

```js
window.Jabba.prompt(prompt); //prompts jabba.js to respond and save your messages to its memory.
//returns the result as a string
```

```js
//"""example"""
console.log(window.Jabba.predict("hello"));
```
