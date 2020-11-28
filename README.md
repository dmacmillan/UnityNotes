## Animation
* When incorporating animation into your character (assuming you are using Unity's built-in `CharacterController`), the `CharacterController.isGrounded` method will stop working and will become `false` unless you start moving forward, even if gravity is being applied.
* The solution is to tweak the `Update Mode` of the `Animator` component on your character to be `Animate Physics`.
* Also make sure that `Apply Root Motion` is checked or true