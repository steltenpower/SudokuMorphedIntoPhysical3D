# Sudoku3D (virtual and physical)

What if you'd turn a (simplified) Sudoku like
<img src="https://i.pinimg.com/736x/29/3d/8d/293d8d80dd44ca8d8f4acc24639d0e40--sudoku-kinder-sudoku-for-kids.jpg">
into a 3D-representation similar to
<img src="https://repository-images.githubusercontent.com/55097385/2ffa4f80-5398-11eb-9f54-8e6aaa2a3aa3">
but with horizontal distances varied a bit to show groups, where each LED is multi-colored to show if Z is the value to fill the X,Y square, maybe with: OFF=no (after tap), GREEN=yes (after hold), ORANGE=undetermined, RED=error

I wonder
- if it's fun to play
- how people cooperate
- if people figure out the logic if you don't tell 'm it's a representation of Sudoku

plus: Sudoku is a nice problem to practice parallel playing/programming/logic on, and this cube a nice thing to shape the rather low-level circuitry around.

It can be somewhat like ...
- virtual: <a href="http://dkobozev.github.io/webgl/led_cube/"><img src="data:image/jpeg;base64,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"></a>
- augmented: [![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/ZI6oJJFgACM/0.jpg)](https://www.youtube.com/watch?v=ZI6oJJFgACM)
- physical: <img src="https://www.playgroundworld.co.za/wp-content/uploads/2019/10/1.8-CLIMBING-CUBE-1.jpg">

more links for implementation:
=========================
- https://stackoverflow.com/questions/14223249/how-can-i-set-the-position-of-a-mesh-before-i-add-it-to-the-scene-in-three-js/29175325
- https://threejs.org/docs/index.html#manual/en/introduction/Creating-a-scene
