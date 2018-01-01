import bs4 as bs
import urllib.request

source = urllib.request.urlopen('https://www.tutorialspoint.com/').read()
soup = bs.BeautifulSoup(source,'lxml')
nav = soup.nav
for url in nav.find_all('a'):

    print(url.get('href'))
    body = soup.body
    print(len(url))
for paragraph in body.find_all('p'):
  print(paragraph.text)
for div in soup.find_all('div', class_='body'):
   print(div.text)
