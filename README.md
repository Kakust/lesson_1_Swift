# lesson_1_Swift

//1

let a: Double = 1
let b: Double = 1
let c: Double = 1

let d = pow(b, 2) - 4 * a * c

if d < 0 {
    print("Нет корней")
}else if d == 0 {
    let x = -b / (2 * a)
    print("Корень уравнения: ", x)
}else {
    let x1 = (-b - d.squareRoot()) / (2 * a)
    let x2 = (-b + d.squareRoot()) / (2 * a)
    print("корни уранвения: ", x1, x2)
}

//2

let sideA: Double = 5
let sideB: Double = 9

let s = sideA * sideB / 2
let h = sqrt(pow(sideA, 2) + pow(sideB, 2))
let p = sideA + sideB + h


//3

var dep: Double = 1000
var per: Double = 6.9

let t = 5

for i in 0..<t {
    dep += (dep * (per * 0.01))
    print("Год: \(i + 1), сумма вклада: \(dep)")
}
