# Command Line Project

```
project -> macOS -> command line tool -> product name
```

# Swift Struct vs Classes

```
struct cannot be inherited and doesn't support encapsulation
let cannot be use`````````````````1 .m,c.d fo``r mutable functions
struct will be destroyed and created wit7+h updated properties when mutable keyword is used.
struct has passed by value whereas classeso ;

[]\ are passed by reference
all variables should be initialized inside classes whether using constructor or while declaration
variables can be uninitialized at struct
```

# Custom View Controller Swift File

```
Right click project directory -> new file -> swift file

shortcuts -> view + enter , ctrl + enter
```

# Custom View Controller Storyboard:

```
Main.storyboard -> new -> view controller
```


# Navigation
```
{
...
performSegue(withIdentifier:"goToResult",sender:self)
}
override func prepare(for segue:UIStoryboardSegue,snder:Any?){
  if segue.identifier == "goToResult" {
      let destinationVC = segue.destination as! ResultViewController
      destinationVC.color = calc.getColor()
  }
}
```

# Add Subviews

```
import UIKit

class SecondViewController:UIViewController{
  override func viewDidLoad(){
    super.viewDidLoad()
    let label = UILabel()
    label.text = "Hello"
    label.frame = CGRed(x:0,y:0,width:100,height:50)
    view.addSubview(label)
  }
}

let secondVC = secondViewController()
secondVC.bmi = "10"
self.present(secondVC,animated:true,completion:null)
```

# 3D view

```
while the app is running , select the three butons icon then drag and move the mobile view
```

# Link two screens

```
Screen 1 -> ^ + click -> drag to -> Screen 2 -> select overlay transition to next screen 
name connection identifier (arrow) as "goToResult
```

# Optionals

```
1. Force unwrapping:

a = nil
let text:String = a!
it will throw run time exception, even through app build succeeds.

2. Check for nil value

if myOptional != nil {
  let text:String = a!
}

3. Optimal Binding

if let safeOptional = optional {
   safeOptionl
}

4. Nil calescing operator

optional ?? defaultValue

5. Optional Chaining

optional?.property
optional?.method()
```


