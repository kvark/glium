# glium

High-level OpenGL wrapper for the Rust language.

```toml
[dependencies.glium]
git = "https://github.com/tomaka/glium"
```

Its objectives:
 - Be 100 % safe to use.
 - Avoid all GL errors. If a GL error is triggered, then it's a bug.
 - Provide all the features that core OpenGL provides.
 - Be compatible with the lowest OpenGL version possible, but still use 4.5 functionnalities if they are available.
 - Be compatible with both OpenGL and OpenGL ES.

## [Link to the documentation](http://tomaka.github.io/glium-docs/glium/)

The documentation contains examples about how to use it.

## Features

Glium has two features: `image` and `gl_extensions`.

 - `image` allows support for the `image` library, which allows to easily textures from different image formats.
 - `gl_extensions` enables functionnalities that are available with OpenGL but not with OpenGL ES. Attempting to use them with OpenGL ES will panic.
