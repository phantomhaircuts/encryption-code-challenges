Keep in mind there are many different solutions to each of these prompts.

# Maskify

```rb
def maskify(cc)
  (cc.length-4).times do |i|
    cc[-5-i] = "#"
  end
  cc
end
```

# Caesar Cipher II (with Bonus)

```rb
def caesar(str, num)
  str.split("")
      .map { |char| char == char[/[a-zA-Z]*/] ? (char.ord + num).chr : char }
      .join()
end
```
