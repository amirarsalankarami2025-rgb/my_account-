public class BinarySearchExample {
    // Binary Search metho
    public static int binarySearch(int[] arr, int target) {
        int left = 0;
        int right = arr.length - 1;

        while (left <= right) {
            int mid = left + (right - left) / 2;

            // If the middle element is the target
            if (arr[mid] == target) {
                return mid;
            }

            // If the middle element is smaller, search the right half
            if (arr[mid] < target) {
                left = mid + 1;
            } 
            // Otherwise, search the left half
            else {
                right = mid - 1;
            }
        }

        // If the element was not found
        return -1;
    }

    public static void main(String[] args) {
        int[] numbers = {2, 5, 8, 12, 16, 23, 38, 56, 72, 91};
        int target = 23;

        int result = binarySearch(numbers, t
