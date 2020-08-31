# Groups, Frames, and Components

```warning
Out of the three, currently only **Groups** are supported by this tool.

**Frames** and **Components** should be changed to **Groups** in order to be converted to useable source code.
```
```warning
Due to API timeout limits, we had to limit our tool to not traverse into multiple nested groups. This limit is currently lifted only for the 'card' and 'form' components which allow other cards and forms to be nested inside. 

Therefore, please try to avoid grouping elements into meaningless groups. Group elements only if they together form a component.
```

Similar to other design tools, groups in Figma allow you to combine multiple elements as a single top-level layer.

In your Figma design, it’s possible that you also used two other functions that can combine many elements: a Frame and a Component. However, these two combination methods are currently not supported within this tool. Only Groups are currently supported and Frames and Components should be changed into groups to ensure their recognition. We plan to add support for Frames and Components in a future update.

Please also note that most of the frontend components are recognized through its name and grouping. Most of the components can only be recognized when they are not nested in another meaningless group. An exception are the 'card' and 'form' components which allow other cards and forms to be nested inside. Most groups without proper naming cannot be recognized and displayed correctly, which is why we recommend to **not use the group in the current version unless you were told so by these guidelines**.
