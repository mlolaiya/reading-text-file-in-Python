# reading-text-file-


#first access the file path
file = open('C:/Users/Mlolaiya/story.txt', 'r')
content = file.read()


def read_file_content(content):
#to read text-file, pass a file name
   content = file.read()

    return content

print(content) #This will print out the text-file

#HOW TO COUNT NUMBER OF OCCURENCE OF WORDS IN PYTHON
def count_words(content):
    counts = dict()
    text = content.split()

    for word in text:
        if word in counts:
            counts[word] += 1
        else:
            counts[word] = 1

    return counts

print(count_words('Once upon a time a psychology professor walked around on a stage while teaching stress management principles to an auditorium '
                  'filled with students. As she raised a glass of water, everyone expected they would be asked the typical glass half empty or glass'
                  ' half full question. Instead, with a smile on her face, the professor asked, How heavy is this glass of water I am holding?'))
