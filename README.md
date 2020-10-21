## Matrix

This package provides a class with basic matrix manipulations

### Install
`npm i @thomas-inst/matrix --save`

### Usage
   
    import {Matrix} from '/your/installation/path/Matrix.js'
    
Create a matrix
    
    let m = new Matrix(20, 10, -1)
    // m contains a matrix of 20 rows x 10 columns 
    // with each element initialized to -1
   
Note: 
* Elements can have anything as their values (string, int, object, ...)
* Rows and columns are numbered starting from 0

Get / Set any value
    

    let v12 = m.getValue(1,2)
    // vl12 ==> -1

    m.setValue(1,2, 123)
    // m.getValue(1,2)  ===> 123
    
Log the matrix to the console

    m.logMatrix()
    
Compare it to other matrix


    let m2 = new Matrix(20, 10, '-')
    m.isEqualTo(m2)
    // ===> false
    
    
Get rows and columns

    let r1 = m.getRow(1)
    let c1 = m.getColumn(1)
    
Add and delete columns

    m.addColumnAfter(1, -2) 
    // m now has 11 columns, with column 2 containing the value -2
    
    m.deleteColumn(2) 
    // m has 10 columns again

Clone it!    
    
    let m3 = m.clone()
    
    
### Development

