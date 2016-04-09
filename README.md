Source code of [mocks-aren-t-stubs mongolian translation](https://www.gitbook.com/book/erheme318/mocks-aren-t-stubs)


# Mocks Aren't Stubs


"Дууриамал объект" гэж жинхэнэ объектуудыг тестлэхийн тулд ашигладаг тусгай оъектуудыг нэрлэдэг бөгөөд нилээдгүй дэлгэрсэн нэршил юм. Ихэнх програмчлалын хэлний орчингууд одоо дууриамал объектуудыг хялбар үүсгэж болох өөр өөрсдийн гэсэн тогтолцоотой болцгоосон. Гэв ихэвчлэн хангалттай ойлгомжтой байдаггүй нэг зүйл нь юу вэ гэхлээр хэдийгээр дууриамал объект нь тестлэх зорилгоор ашиглагддаг нэг хэлбэрийн тусгай объект боловч, мөн нөгөөтэйгүүр тестлэх өөр нэг загварчлалын аргыг бий болгосон байдаг. Энэхүү нийтлэлээр би та бүхэнд дууриамал объект хэрхэн ашиглагддаг, үйлдэл шалгах явцыг (behavior verification) хэрхэн дэмждэг болон мөн хөгжүүлж, дэмжиж буй бүлгэмийн залуус хэрхэн өөр нэг тестлэх загварыг хөгжүүлж байгаа талаар тайлбарлах болно.

Би энэхүү "дууриамал объект" гэх нэршлийг анх хэдэн жилийн өмнө Extreme Programming (XP) бүлгэмийн нөхдүүдээс дуулж билээ. Түүнээс хойш энэхүү дууриамал объектууд миний сонирхлыг улам ихээр татах болсон. Нэг шалтгаан юу гэхлээр дууриамал объектуудын хөгжүүлэлтийг авч явж байсан нилээдгүй хөгжүүлэгчид надтай хамт ThoughtWorks-д хамт ажиллаж байсантай холбоотой байх. Нөгөө нэг шалтгаан нь юу гэвэл би энэхүү ойлголтыг XP -ын нөлөөлөлтэй тестлэх аргад тулгуурласан зохиол бүтээлүүдээс их харж байсантай ч холбоо байх.

Гэвч би энэхүү дууриамал объектуудын талаар муу тайлбарласан зүйлүүдтэй олонтаа таардаг. Ялангуяа хүмүүс эдгээр дууримал объектуудыг хэлтэрхий (stub) тай хольж хутгаад байдгыг би мэднэ. Яагаад хольж хутгаад байдгыг нь ч би сайн мэднэ - учир нь би өөрөө ч нэг хэсэг мөн тэгж харж байлаа. Харин тэдгээр дууриамал объектын хөгжүүлэгч нартай хийсэн ярилцлагууд намайг өчүүхэн ойлголтоос минь бүр цөм рүү нэвтрэн орж, нарийн мэдэхэд минь их тус болсон.

>**Тайлбар**:
Stub - тестэнд объектын зөвхөн зарим методын үйлдлийг дууриалгах зорилгоор ашиглагддаг тул хэлтэрхий объект гэж нэрлэсэн

Энэ ялгаа нь үнэндээ бол хоёр тусдаа ялгаатай зүйлүүд байгаа юм. Нэг талдаа тестийн үр дүнг хэрхэн батлах аргуудад ялгаа бий: объектын төлвийг батлах (state verification) болон объект хоорондын харьцаж буй үйлдлийг батлах (behavior verification). Нөгөөтэйгүүр тестлэх, загварчлах хоёрын хоорондоо хэрхэн нөлөөлж байгаа арга барил философи -д нь ялгаа бий. Энэ ялгааг би доор тайлбарлахдаа Тестээр хөтлөгдөх хөгжүүлэлт (Test Driven Development) -ын сонгодог болон дууриамал аргууд гэж нэрлэсэн болно.
