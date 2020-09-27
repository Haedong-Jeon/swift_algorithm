# contains() 메소드 없이 한 문자열이 다른 문자열을 포함하는지 알아보기.     
   
## Solution    

```swift
extension String {
    func solution2(_ string: String) -> Bool {
        return self.range(of: string, options: NSString.CompareOptions.caseInsensitive) != nil
    }
}
```       
**range(of: ) 메소드**를 이용하면 간단하다. range(of:)메소드는 String 클래스의 메소드다.      
이 메소드는 **자신 안에서 인자로 전달된 문자열이 어디에 있는지 찾아 반환**한다. 만약 존재하지 않는다면 nil을 반환한다.

