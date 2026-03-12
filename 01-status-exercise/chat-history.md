# Chat History — status.js Exercise

---

## Prompt 1

> Write a Node.js script called status.js that prints a status report to the terminal when run with `node status.js`.
>
> The output should look exactly like this:
> ```
> Status: OK
> Time: 2024-01-15T10:30:00.000Z
> ```
>
> Requirements:
> - Use console.log to print each line
> - Get the current time using `new Date().toISOString()`
> - No npm packages — only built-in Node.js features

### Code written — `status.js`

```js
console.log("Status: OK");
console.log("Time: " + new Date().toISOString());
```

### Output

```
Status: OK
Time: 2026-03-12T02:25:22.451Z
```

---

## Prompt 2

> Now add a third line to the output that shows how long Node has been running, using process.uptime(). Round it to 2 decimal places. The new line should look like:
>
> `Uptime: 0.05s`

### Code written — `status.js`

```js
console.log("Status: OK");
console.log("Time: " + new Date().toISOString());
console.log("Uptime: " + process.uptime().toFixed(2) + "s");
```

### Output

```
Status: OK
Time: 2026-03-12T02:26:11.566Z
Uptime: 0.03s
```

---

## Prompt 3

> Add a fourth line showing memory usage in MB using process.memoryUsage().heapUsed

### Code written — `status.js`

```js
console.log("Status: OK");
console.log("Time: " + new Date().toISOString());
console.log("Uptime: " + process.uptime().toFixed(2) + "s");
console.log("Memory: " + (process.memoryUsage().heapUsed / 1024 / 1024).toFixed(2) + "MB");
```

### Output

```
Status: OK
Time: 2026-03-12T02:27:23.554Z
Uptime: 0.03s
Memory: 3.70MB
```

---

## Prompt 4

> Dump the output of this chat into a MD file with all the outputs.

Created this file: `chat-history.md`
