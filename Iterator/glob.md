glob
====

    import glob
    for filename in glob.glob('*.jpg'):
        print(filename)
    
**현재 디렉토리에서 확장자가 jpg인 파일만 모아서 출력한다.**
    
    import glob
    for filename in glob.iglob('**/*.jpg', recursive = True):
        print(filename)

**재귀적으로 현재 폴더의 모든 하위 폴더까지 탐색하여 확장자가 .jpg인 파일을 출력한다.**

    import glob
    for filename in glob.iglob('ABCD/**/*.jpg', recursive = True):
        print(filename)
        
**ABCD 폴더를 재귀적으로 돌며 jpg파일을 출력한다.**
    
    
