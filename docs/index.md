# Crater

> A type safe superset of Lua — without losing what makes Lua special.

---

## What is Crater?

Crater is a typed language that compiles down to Lua.  
It was made to feel like Lua, but every variable and function has a type — giving you:

- ✅ Early error detection (catch bugs before runtime)
- ✅ Safer large-scale code
- ✅ Better editor and tooling support

You don't lose Lua's simplicity — you just gain structure.

---

## A basic example

In Lua you might write:

```lua
local function greet(name)
    print("Hello, " .. name .. "!")
end

greet("world")
```

In Crater, you simply specify types to be enforced:

```lua
local function greet(name: string): void
    print("Hello, " .. name .. "!")
end

greet("world") -- ✅ Type-checked
greet(123)     -- ❌ Error, expected string, got number
```

## Why Crater?

Lua is great for quick scripting and flexibility.  
Crater is for when you want the same Lua spirit, but with the **safety and clarity** of a modern language.

That way you can focus on your project without the need to keep track of the type of every variable you are using — no more type checks at the top of functions.
