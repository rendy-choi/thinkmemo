# thinkmemo
npx prisma migrate diff --from-schema-datamodel prisma/schema.prisma  --to-schema-datasource prisma/schema.prisma --script
npx prisma migrate resolve --applied 20250721012457_add_friend_share_feature

# 프로젝트 루트로 이동

cd /mnt/c/Users/studi/mirim/project/mirim-tax.io

# 스키마를 데이터베이스에 직접 푸시 (개발 환경용)

npx prisma db push

# Prisma Client 재생성

npx prisma generate

## 프로덕션 데이터가 있다면


# 프로젝트 루트로 이동

cd/mnt/c/Users/studi/mirim/project/mirim-tax.io

# 현재 스키마 상태로 새로운 마이그레이션 생성

npxprismamigratedev--namereinit_schema

# Prisma Client 재생성

npxprismagenerate



디비 백업 순서 

 tb_company

tb_invited

tb_native_device_info

tb_member

최기선 / chlrltjs1@hanmail.net
정지윤 / jy970508@nate.com
김유민 / ym0402k@naver.com
최초희 / uniquechoa@naver.com
오은석 / ohes920412@naver.com
박성민 / sungmin5307@kakao.com
입니다! 


# 스키마 변경사항을 마이그레이션으로 생성하고 즉시 적용
npx prisma migrate dev --name describe_your_changes

# 예시:
npx prisma migrate dev --name remove_gift_table
npx prisma migrate dev --name add_friend_share_feature
