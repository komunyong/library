# Python

## Basic Usage

### Top-level script environment: __main__

Example condition to execute this code only when it get execute by script or command `python -m`, its not run when imported.
```python
if __name__ == "__main__":
  # execute only if run as a script
  main()
```

References: https://docs.python.org/3/library/__main__.html

### **args, **kwargs
**args (for all arguments), **kwargs (for all key-value argumensts): It used as module input when you don't know how many inputs that you want.

```python

# Example **args
def print_everything(*args):
  for count, thing in enumerate(args):
    print( '{0}. {1}'.format(count, thing))

print_everything('apple', 'banana', 'cabbage')

# output
# 0. apple
# 1. banana
# 2. cabbage

# Example **kwargs
def table_things(**kwargs):
  for name, value in kwargs.items():
    print( '{0} = {1}'.format(name, value))

table_things(apple = 'fruit', cabbage = 'vegetable')

# output
# cabbage = vegetable
# apple = fruit
```

Reference: https://stackoverflow.com/questions/3394835/args-and-kwargs


## Alias python3 and pip3 usage

Edit last line of `~/.bashrc` or `~/.zshrc` with

alias python=python3
alias pip3=pip

then execute
  source ~/.zshrc or source ~/.bashrc