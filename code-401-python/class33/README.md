# Class 33
## Next- Forms and Conditional Rendering 

### Custom Hooks
Build a Hook
In the following code, we are fetching data in our Home component and displaying it.

We will use the JSONPlaceholder service to fetch fake data. This service is great for testing applications when there is no existing data.

To learn more, check out the JavaScript Fetch API section.

### Lifting State Up

In React, sharing state is accomplished by moving it up to the closest common ancestor of the components that need it. This is called “lifting state up”. We will remove the local state from the TemperatureInput and move it into the Calculator instead.

If the Calculator owns the shared state, it becomes the “source of truth” for the current temperature in both inputs. It can instruct them both to have values that are consistent with each other. Since the props of both TemperatureInput components are coming from the same parent Calculator component, the two inputs will always be in sync.
### Thinking in React
1. Looking at the bigger picture
There’s always a big emphasis on creating React Components which can be reusable, maintainable and easy to test. For beginners it’s always very tempting to dump all the rendering logic into one big component. I think that’s how we all started to learn React. But, as our mind power grows, we can see this is not how it’s meant to be done.
2. React PropTypes — your best friend
I personally love React’s built-in typechecking feature as it gives me confidence about getting my components to render properly. But, I have seen beginner developers abusing it to the level where its values is completely lost.

3. Understanding setState little further
You might have heard lots of talk about which React lifecycle hook to be used for calling setState. As this function is the core of React, it’s important to understand what happens when you call this function.

4. One job per component
You can embed few lines of logic in your render function which is alright. But, I always find it easy to divide the logic and delegate that to other component if render function starts to look messy. 

5. Using ComponentWillUnmount wisely
You might have encountered an error in console saying “can’t call setState on unmounted component” and have spent some time struggling to find the root cause. It’s frustrating.
### Memoization in React

In programming, memoization is an optimization technique that makes applications more efficient and hence faster. It does this by storing computation results in cache, and retrieving that same information from the cache the next time it's needed instead of computing it again.

In simpler words, it consists of storing in cache the output of a function, and making the function check if each required computation is in the cache before computing it.

A cache is simply a temporary data store that holds data so that future requests for that data can be served faster.

Memoization is a simple but powerful trick that can help speed up our code, especially when dealing with repetitive and heavy computing functions.