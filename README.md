1) I think it would be best to put the tests in a GitHub action that runs whenever code is pushed. This way, you could always ensure that your code is working in the final version, as you'd be alerted before you pushed any code that broke it. This could also help you bugfix and catch errors before they go to the main project.

2) No, an end-to-end test is meant to test user interactions with the entire system. Testing if a function returns the right value would be better to do with a unit test, as you only need to test one part of the code.

3) Navigation mode analyzes the page right after it loads. Snapshot mode analyzes the page in its current state.

4) There are improvements we could make to performance since it's only at 87 right now. Some of the best would be minifying and removing unused JavaScript, fix delayed rendering, and avoid chaining critical requests together so the page can load faster.
