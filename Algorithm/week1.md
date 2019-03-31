## 第一周
- twoSum

		func twoSum(nums []int, target int) []int {
            var result = make([]int, 2)
            length := len(nums)
            if length > 1 {
                for i := 0; i < length-1; i++ {
                    for j := i+1; j < length; j++ {
                        if target == nums[i] + nums[j] {
                            result[0] = i
                            result[1] = j
                            return result
                        }
                    }
                }
            }

            return result
        }
