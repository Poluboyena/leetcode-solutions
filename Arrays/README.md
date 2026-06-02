Array problems

class Solution:
    def kWeakestRows(self, mat: List[List[int]], k: int) -> List[int]:
        lis=[]

        for i in range(len(mat)):
            c=0
            for val in mat[i]:
                if val==1:
                    c+=1
            lis.append((c,i))
        lis.sort()

        result=[]
        for c,i in lis:
            result.append(i)
        return result[:k]        
        return lis





        
