# How to call a function from another script

You can call funtions from other scripts like this:

```c#
using UnityEngine;

public BigRedButton btn;

public class ButtonPusher : MonoBehaviour
{
  public void Update()
  {
     if(time_to_push_button)
     { 
        btn.Push();
     }
  }
}
```

if some there exists a gameobject with a script called BigRedButton attached to it. The script might look like this:

```c#
using UnityEngine;
public class BigRedButton : MonoBehaviour
{
  public void Push()
  {
     Debug.Log("That was easy");
  }
}
```

