Array{Int64}(undef, 3) (fills array with random)

] goes to package manager
  status for checking 
? for help
; for shell
    
 apropos
 apropos("vector")
 
 
 using OhMyREPL
 
 s1 = "this is a string"
 
 s1[end]
 
 parse(type, str; base)
 
 supertype, subtype
 
 push!(a2, 3)
 
 fill
 
 fill(value, dims::Tuple)
 Create an array of size dims with every location set to value.
 
 
 
 reshape
 
 Julia is columnwise, [column, row]
 
 e = [i for i in 1:10] gives you vector from 1 to 10 
 
collect(element_type, collection)
 
findall (x -> x > 3, array)
gives you all indices where x > 3

findmax, findmin
 
anonymous function = function without name
 
 
 rand makes random numbers
 e.g. rand(3,2) gives 3x2 matrix

struct constructs objects with fields

struckt T1
x
y
end



t1 = T1(3, 4) 

 
acces fields by t1.x

mutable struct T2
x::Float64
y::Int
end

now you can change values

for loops:
for i in ....
bla bla
end


functions
function f2(x, y; z=1, w=2)
x + y + z + w

f2(2, 3) uses default values for z and w
f2(2, 3, z=3) you have to name z to pass it

function f2(x::Int, y::Int; z=1, w=2)
__creates new method for same function__


Dict
keys()
values()

for tabular data:
package DataFrames

columns of different types
df.A (column A)

df[:, :A] (also column A)
df[row, column]

push! also works here


CSV package
CSV.read(file, DataFrame)

open("file", "w") do f3
for i in 1:10
println(f3, i)
end
end

parse.(Int, j)
adding a point... so you can use a list?


Modules:
include()
  functions.jl
  typeof.jl
using...

environments and modules??


 Revise package for importing module files
  includet
