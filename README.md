# Assignment-01-may-12-2o22
class Solution:
    def isValid(self, s: str) -> bool:
        while(True):
            if "()" in s:
                s = s.replace("()","")
            elif "[]" in s:
                s = s.replace("[]","")
            elif "{}" in s:
                s = s.replace("{}",'')
            else:
                return not s
