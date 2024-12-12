
BAT/IT/2022/P/64

public class StrictlyIncreasingArray {
    public static boolean isStrictlyIncreasing(int[] arr) {
        for (int i = 1; i < arr.length; i++) {
            if (arr[i] <= arr[i - 1]) {
                return false;
            }
        }
        return true;
    }

    public static void main(String[] args) {
        int[] inputArray = {1, 3, 5, 7, 9};
        boolean result = isStrictlyIncreasing(inputArray);
        System.out.println(result); // Output: True
    }
}