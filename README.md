mahonia
=======

 character-set conversion library implemented in Go.

 Mahonia is a character-set conversion library implemented in Go.
 All data is compiled into the executable; it doesn't need any external data files.

 based on http://code.google.com/p/mahonia/

install
-------

	go get github.com/nzlov/mahonia

example
-------

	package main
	import "fmt"
	import "github.com/nzlov/mahonia"
	func main(){
	  enc:=mahonia.NewEncoder("gbk")
	  //converts a  string from UTF-8 to gbk encoding.
	  fmt.Println(enc.ConvertString("hello,世界"))  
	}

