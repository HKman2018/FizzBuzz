# FizzBuzz Test
* case1: input: 9, expect output : Fizz
* case2:input:10,ecpect output: Buzz
* case3:input:15,ecpect output:FizzBuzz
* case4:input:7,ecpect output:7

# Spec.js
```var should = chai.should()

describe('FizzBuzz test', function () {
  it('[case1]: input: 9, expect output : Fizz', function () {
    const result = fizzBuzz(9)
    result.should.be.equal('Fizz')
  })
  it('[case2]:input:10,ecpect output: Buzz', function () {
    const result = fizzBuzz(10)
    result.should.be.equal('Buzz')
  })
  it('[case3]:input:15,ecpect output:FizzBuzz', function () {
    const result = fizzBuzz(15)
    result.should.be.equal('FizzBuzz')
  })
  it('[case4]:input:7,ecpect output:7', function () {
    const result = fizzBuzz(7)
    result.should.be.equal(7)
  })
})```

# Test.js
```function fizzBuzz(num) {
  let str = ''
  if (num % 3 === 0) {
    str += 'Fizz'
  }
  if (num % 5 === 0) {
    str += 'Buzz'
  }
  if (str != '') {
    return str
  } else {
    return num
  }
}```
