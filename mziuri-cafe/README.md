# მზიური / Mziuri Cafe

პატარა თანამედროვე თბილისის კაფეს ერთგვერდიანი responsive დემო.

## რას შეიცავს

Hero, About, Menu, Gallery, Location/Hours, Contact და Footer. მობილური ნავიგაცია, მენიუს კატეგორიების ფილტრი, კლავიატურით სამართავი ფოტო გალერეა, reduced-motion მხარდაჭერა. ქართული კონტენტი და SEO მეტამონაცემები.

Frontend: HTML/CSS/JavaScript — framework-ის გარეშე. Backend: Node.js-ის პატარა სტატიკური სერვერი, გარე დამოკიდებულებების გარეშე. მონაცემთა ბაზა და API გასაღებები საჭირო არ არის.

## გაშვება

დააყენე Node.js 22 ან ახალი ვერსია. პროექტის საქაღალდეში:

```bash
npm ci
npm start
```

გახსენი http://localhost:3000. შემოწმება: `npm run check`.

## GitHub-ზე ატვირთვა

GitHub-ზე შექმენი ცარიელი repository სახელით `mziuri-cafe` (README-ის დამატების გარეშე). პროექტის საქაღალდეში გაუშვი:

```bash
git init -b main
git add .
git commit -m "Build Mziuri Cafe responsive demo"
git remote add origin https://github.com/YOUR_USERNAME/mziuri-cafe.git
git push -u origin main
```

`YOUR_USERNAME` შეცვალე შენი GitHub მომხმარებლის სახელით. Windows-ზე გამოიყენე Git Bash ან VS Code-ის terminal. ალტერნატივა: GitHub Desktop → Add local repository → Publish repository.

## Railway-ზე გამოქვეყნება

1. Railway-ში შექმენი New Project და აირჩიე Deploy from GitHub repo.
2. აირჩიე `mziuri-cafe` repository. პროექტის root directory დატოვე `/`.
3. `railway.json` განსაზღვრავს Railpack-ს, `npm start` ბრძანებას და `/health` შემოწმებას.
4. დასრულების შემდეგ გახსენი Service → Settings → Networking → Generate Domain.
5. გახსენი Railway-ის გენერირებული ბმული. GitHub-ზე მომავალი push-ები დაკავშირებულ branch-ზე ავტომატურ redeploy-ს იწვევს.

სერვერი უსმენს `0.0.0.0`-ს და Railway-ის `PORT` ცვლადს; PORT-ის ხელით დამატება საჭირო არ არის. ფიქსირებული ხარჯი აქ არ არის მითითებული — Railway-ის მიმდინარე გეგმა/მოხმარება გადაამოწმე ანგარიშში.

ოფიციალური ინსტრუქციები:
- https://docs.railway.com/quick-start
- https://docs.railway.com/guides/express
- https://docs.railway.com/guides/public-networking

## რედაქტირება

- `public/index.html` — ქართული ტექსტები, მენიუ, ფასები, საათები, კონტაქტები.
- `public/styles.css` — ფერები, დაშორებები და მობილურის განლაგება.
- `public/script.js` — ნავიგაცია, ფილტრი, ფოტოს გადიდება.
- `public/assets/` — ფოტოები და favicon.
- `server.js` — სტატიკური ფაილების სერვერი.
- `.github/workflows/check.yml` — GitHub Actions-ის სინტაქსის შემოწმება.

## დემოს მონაცემები

„მზიური“ გამოგონილი კაფეს კონცეფციაა. მენიუ, ფასები და საათები დემოსთვისაა. რუკის ბმული მიუთითებს რეალურ მზიურის პარკს და არა დადასტურებულ კაფეს მისამართს. კონტაქტები დასამატებელი ველებია; ყალბი ტელეფონი და სოციალური ანგარიში არ გამოიყენება. კონტაქტის ფორმა და შეკვეთების სისტემა არ არის ინტეგრირებული.

გამოქვეყნებამდე ჩაანაცვლე ზუსტი მისამართი, სამუშაო საათები და მენიუ. დაამატე რეალური `tel:`, `mailto:` და Instagram ბმულები. დემოს მინაწერი დატოვე მანამ, სანამ ინფორმაცია ნამდვილ ბიზნესს არ ეკუთვნის.

ფოტოები შექმნილია AI-ით როგორც ორიგინალური ილუსტრაციული კონცეფციები: მზით განათებული თანამედროვე კაფე; კაპუჩინო და კრუასანი; ავოკადოს ტოსტი. ისინი რეალური „მზიურის“ ფოტოსურათები არ არის.
