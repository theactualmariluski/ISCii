# ISCii
Go library to make dinamic ascii, full control of the standard screen, menus, banners with FIGlet and more.
## Instalation
You can install ISCii with go, like always
```bash
  go get ISCii
```
## Usage
To use ISCii **you need to make objets**
You can make a objet with: ```var myObject = ISCii.object("how it looks")``` replace "how it looks" to how you want it to look, you can also use FIGlet like on the example bellow:
```golang
package main //put your package, it doesn't matter
import "ISCii"

func main() {
  var stdScr = ISCii.stdsct() // gets the standard screen (terminal)
  var myObjet := ISCii.object(ISCii.figlet("ISCii Rocks!") //creates a FIGlet text as an object
  var myInstance myObject.put(0,0) //creates a insance
  for {
    myObject.move(myObject,1) // moves myObject
  }
}
```
