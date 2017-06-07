# go_notes

//Types
// boo. string int, int8, int16, int32, etc
//Other types
// Array, Slice, Struct, Pointer, Map
}
// declare variable
// shorthand only used inside function
// var has zero value

//Basic Declarartion

//var message string
//message = "Hello Go World"
// var a, b, c int = 1, 2, 3 or var a, b, c = 1, 2, 3 or a, b, c := 1, 2, 3

//Pointer
// Pointer point to memory location
// You can access other variable with pointer
// * = pointer holds memory value
// & = Gives the memory value
// message  := "Hello Go World"

// var greeting * string = &message
// *greeting = "hi"
// ex) above sets the pointer to string and returns memory value of the message

// if you print (message, greeting) it will come out "Hello Go World" and Memeory value
// if you print *greeting it will give "Hello Go World"
// if you set * greeting = "hi" when you print (message, *greeting) it will return hi hi

//No classes in Go!
//type 
// type salutation struct {
// 	name string
// 	greeting string

// }
// func main () {
// 	var s = salutation{}
// 	s.name = "bob"
// 	s.greeting = "hello there"
// }


//const
// const {
// 	PI = 3.14
// 	Language = "Go"
// 	A = iota
// 	B = iota
// 	C = iota
// }

//function
// type Salutation struct {
// 	name string
// 	greeting string
// }
// func Greet(salutation Salutation) {
// 	fmt.Println(salutation.name)
// 	fmt.Println(salutation.greeting)
// }

// func main() {
// 	var s = Salutation{"Bob", "hello"}
// 	Greet(s)
// }
// Creating Multiple returns
// func CreateMessage(name, greeting string) (string, string) {
// 	return greeting + " " + name, "HEY!" + name
// }

//For
//Ranges
//Types of Ranges: Array or slice, String, Map, Channel
// for i, s := range salutation {

// }
// The above will loop through salutation



//putting two arrays together
// mySlice := []int{1,2,3}
// mySlice2 : = []int{4,5,6}
// mySlice = append(mySlice, mySlice2...) if you want add extra append(mySlice, "hello")
// which gets you [1,2,3,4,5,6]

//empty array
// mySlice := []int{}
// mySlice := make([]int, 0)

// mySlice := make([]int, 0)
// for i := 0; i < 10; i++ {
// 	mySlice = append(mySlice, i)
// 	fmt.Println(len(mySlice))
// }

// for i := 0; i <= 100; i++ {
// 	fmt.Println(i)

// myArr := [...]int{1,2,3,4}
// for i := 0; i < len(myArr); i++ {
// 	fmt.Println(myArr[i])
// }

//const (
// 	first = iota
// 	second
// 	third
// )
// iota auto increments so first prints 0, second 1, third 2

// while
// i := 0
// for i < 10 {
// 	fmt.Println(i)
// 	i++
// }

// Infinite Loop
// i := 0
// for {
// 	fmt.Println(i)
	// if i >= 10 {   You can put condition to break the infinite loop
	// 	break
	// }
// 	i++
// }

//continue makes it so if condition isn't true it will go back to loop

// String

// Double quote will give you the string it self
// Single quote will give you rune code which is int32

// array
// var s []int
// var x [58]string
// len(x)
// myArray := [...]int{42,27,99}
// myArray : = [3]int

//slice
// mySlice := myArray[1:]
// mySlice := myArray[:]
// mySlice := make([]int, 100)
//map
// myMap := make(map[int], string)
//reference type: Pointing to structure(pointers).
// var myMap = make(map[string]string)
