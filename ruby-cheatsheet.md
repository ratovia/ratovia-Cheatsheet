# 標準出力
## 改行なし
```
print "hello world"
```
## 改行あり
```
puts "hello world(puts)"
```
## データタイプで出力
```
p "hello world(p)"
```

# コメント
    =begin
    comment
    comment
    =end
    # コメント

# 標準入力
```
A,B = gets.split.map(&:to_i)
print A+B,' ',gets
```

# 配列
```
sales = [5,8,4,"res"]
array = Array.new(3){ Array.new(3) }
p sales[1]
p sales[0..2]
p sales[0...2]
p sales[-1] # last
p sales[1,2] # 1 kara 2ko
p sales.push(100)
sales << 100 << 102
sales = {"taguchi" => 200,"fujii" => 300} #hash
p sales["taguchi"]

sales = {:taguchi => 200, :fkoji => 300}
p sales[:taguchi]
```

# 型変換
```
a = 10
b = "5"
p a + b.to_i
p a + b.to_f
p a.to_s + b
h = {taguchi:100,fkoji:200}
p h.to_a.to_h
```

# if文
```
score = 80
if score > 60
	puts "OK!"
elsif score > 40
  puts "SOSO..."
else
	puts "NG!"
end
```
# switch文
```
signal = "red"

case signal
when "red"
	puts "stop!"
when "green"
	puts "GO"
else
	puts "wrong"
end
```

#loop
```
3.times do |i|
	puts "#{i}: hello"
end

i = 0
while i < 3 do
	puts "#{i}: hello"
	i += 1
end

for i in 0..2 do
	puts i
end

["red","blue","pink"].each do |color|
	puts color
end
```

# 関数
```
def sayHi(name)
	puts "hello" + name
	s = "hello" + name
	return s #return
#	s #return
end

sayHi("Tom")
sayHi("Bob")

greet = sayHi("Sub")
puts greet

```

# class
```
class User
	@@count = 0
	def initialize(name)
		@name = name
		@@count += 1
	end

  def name
		return @name
	end

	def setName(newName)
		@name = newName
	end

  attr_accessor :name
	def sayH
		puts "hello, my name is #{@name}"
	end
	def User.sayHello # class method
		puts "hello from User class(#{@@count} users)"
	end

end

User.sayHello()
tom = User.new("TOm")
tom.sayH()
User.sayHello()


class SuperUser < User
	def shout
		puts "HELLO from #{@name}!"
	end
end

bob = SuperUser.new("Bob")
bob.shout();
p tom.name
tom.name = "Tom"
```

# Method type
! destory method  
? true or false
