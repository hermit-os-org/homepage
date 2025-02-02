---
layout: default
---

[Hermit](http://hermit-os.org) is a [unikernel](http://unikernel.org) targeting a scalable and predictable runtime for high-performance and cloud computing.
Unikernel means, you bundle your application directly with the kernel library, so that it can run without any installed operating system.
This reduces overhead, therefore, interesting applications include virtual machines and high-performance computing.

The kernel is able to run [Rust](https://github.com/hermit-os/hermit-rs) applications, as well as [C/C++/Go/Fortran](https://github.com/hermit-os/hermit-playground) applications.

# Background

**Hermit** is a rewrite of HermitCore in [Rust](https://www.rust-lang.org) developed at [RWTH-Aachen](https://www.rwth-aachen.de).
HermitCore was a research unikernel written in C ([libhermit](https://github.com/hermit-os/libhermit)).

The ownership  model of Rust guarantees memory/thread-safety and enables us to eliminate many classes of bugs at compile-time.
Consequently, the use of Rust for kernel development promises fewer vulnerabilities in comparison to common programming languages.

The kernel and the integration into the Rust runtime are entirely written in Rust and do not use any C/C++ Code.
We extended the Rust toolchain so that the build process is similar to Rust's usual workflow.
Rust applications that use the Rust runtime and do not directly use OS services are able to run on Hermit without modifications.


## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
