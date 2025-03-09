class Solution:
    def merge(self, nums1: List[int], m: int, nums2: List[int], n: int) -> None:
        """
        Do not return anything, modify nums1 in-place instead.
        """
        n1p = m - 1
        n2p = n - 1
        rp = m + n - 1

        while (rp >= 0):
            if (n1p < 0):
                nums1[rp] = nums2[n2p]
                rp -= 1
                n2p -= 1
            elif (n2p < 0):
                nums1[rp] = nums1[n1p]
                rp -= 1
                n1p -= 1
            elif (nums1[n1p] > nums2[n2p]):
                nums1[rp] = nums1[n1p]
                rp -= 1
                n1p -= 1
            else:
                nums1[rp] = nums2[n2p]
                rp -= 1
                n2p -= 1
