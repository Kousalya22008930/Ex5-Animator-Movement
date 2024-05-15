# Ex5-Animator-Movement
### Aim:
To develop a animator movement for a player using unity.


### Algorithm:
Step 1: Import necessary models.

Step 2: Right-click -> Create -> Animator Controller.

Step 3: Open Animator window, define states (Idle, Run, Jump, etc.).

Step 4: Use keyframes or Unity's Animation tools to animate transitions between states.

Step 5: Drag Animator Controller to the GameObject in the Inspector.
### Program:
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class script : MonoBehaviour
{
    public Animator animator;
    public float inx;
    public float iny;

    // Start is called before the first frame update
    void Start()
    {
        animator = this.gameObject.GetComponent<Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        inx = Input.GetAxis("Horizontal");
        iny = Input.GetAxis("Vertical");
        animator.SetFloat("inx",inx);
        animator.SetFloat("inY",iny);
    }
}
```
## Output:
## Idle position:
![image](https://github.com/Kousalya22008930/Ex5-Animator-Movement/assets/119389108/db8678d9-76f0-4c9b-8ab2-3cbead6219c3)
## Crouch position:
![image](https://github.com/Kousalya22008930/Ex5-Animator-Movement/assets/119389108/b2d07a3f-4797-40da-9277-9d60bfef9595)
## Walking:
![image](https://github.com/Kousalya22008930/Ex5-Animator-Movement/assets/119389108/b476bca9-21c8-416c-ba5c-505583be2cbb)

## Result:
An animator movement for a player using unity is developed successfully.

